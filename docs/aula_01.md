---
title: O que é e qual o propósito do Temporal?
description: Vamos entender o porque o Temporal é tão usado e amigável ao desenvolvedor
---

# O que é e qual o propósito do Temporal?


---
Objetivos dessa aula:

- Entender o que é o Temporal e qual seu propósito
- Mostrar as nomeclaturas do Temporal (Workers, workflows, activities, etc.)
- Iniciando o Temporal a partir de um docker compose
- Iniciando o SDK do Temporal com Typescript
- Execução do primeiro "Hello, World!" com Temporal, usando Workflows e Activities
---

Nesta aula, iniciaremos nossa jornada no entedimento do Temporal e na construção de uma Worker rodando de verdade. Partiremos do início: principais dores que as empresas tem, motivo das empresas utilizarem Temporal.io, o que ele facilita na vida do desenvolvedor e principais nomeclaturas que precisamos entender para iniciar.

Após isso, configuraremos o ambiente do Temporal utilizando o docker-compose, mostrando a UI do Temporal Server. Em seguida, mostrarei como montar um ambiente apropriado para criar um worker utilizando o Temporal SDK do Typescript. E então, finalmente, criaremos nosso primeiro "Hello, World!" a partir de um Workflow.

## Propósito do Temporal

O Temporal é uma plataforma de orquestração de execuções distribuídas e duráveis que permite o desenvolvimento de aplicações resilientes e escaláveis. Ele fornece um modelo baseado em workflows para gerenciar tarefas assíncronas, garantindo confiabilidade, consistência e tolerância a falhas sem que nós, pobres desenvolvedores, precisemos lidar com complexidades como retries, timeouts e recuperação de falhas NA MÃO.

O principal propósito do Temporal é simplificar a construção de sistemas distribuídos ao fornecer uma maneira fácil de definir quais execuções devem ser realizadas. O servidor do Temporal gerencia essas execuções, garantindo que tarefas sejam concluídas mesmo em cenários de falha, reinicialização ou indisponibilidade temporária dos serviços.

Vamos imaginar então que somos uma fintech que processa pagamentos para lojistas e precisamos garantir que todas as transações sejam concluídas com sucesso. Mas de vez em quando quando ninguém está olhando, final de semana, ocorrem falhas na comunicação com o banco ou então o sistema trava antes de confirmar a transação.

Usando Temporal, nossa empresa pode garantir que cada pagamento **SERÁ** concluído, mesmo se houver falha no sistema ou reinicialização do servidor. A execução do Temporal retomará a transação do ponto de falha, retentando só a parte que deu falha e seguindo o resto da execução normalmente, sem risco de pagamentos duplicados ou não processados. Isso é o que a gente busca atacar: garantia de execução como se nada tivesse acontecido.

## Nomeclaturas importantes

### Activities

Uma Activity é o ponto mais simples disso tudo, ela é basicamente apenas uma função ou uma tarefa que faz parte de um Workflow. Normalmente, são operações que envolvem chamadas externas, como acessar um banco de dados, enviar um e-mail ou chamar uma API.

Quando desenvolvendo Activities, projete elas imaginando que elas  podem falhar, mas que o Temporal automaticamente vai gerenciar as retries e timeouts para garantir que sejam concluídas.

### Workflows

Um Workflow no Temporal é a unidade principal de orquestração de processos. Ele define um fluxo de execução que pode incluir várias etapas e chamadas assíncronas. Os Workflows podem pausar e continuar do ponto onde pararam, mesmo após falhas ou reinicializações do sistema.

Pense em um Workflow como uma passo-a-passo das Activities. Quando ele for montado, ele deve ser imaginado como um processo que precisa ser recomeçado todo do zero em caso de falha.

### Workers

Um Worker no Temporal é, de forma simples de se explicar, o nosso código. Ele é responsável por registrar no Temporal Server os nossos Workflows e Activities. Ele deve possuir um ID específico chamado **task-queue** que gerará uma fila no Temporal Server em que Workers idênticos (como no caso de necessário escalar réplicas por exemplo) poderão se inscrever. A task-queue é gerada quando você conecta o Worker ao Temporal Server.

Nele há uma série de configurações que poderão ser abordados no futuro, mas trabalharemos primeiro com o básico para não nos embaralharmos muito.

*PS: Workers só podem ser registrados se eles possuirem ao menos uma Activity*

### Namespaces
Um Namespace no Temporal é uma área separada onde todos os componentes operam de maneira isolada, permitindo que diferentes aplicativos ou serviços dentro do mesmo cluster do Temporal não interfiram entre si. Eles são separados por nomes diferentes. Nesse curso, não vamos nos aprofundar em namespaces, pois usaremos a auto-gerada.

Para criar uma namespace específica no Temporal iniciado pelo docker compose desse curso, devemos usar o comando:

```sh
docker exec -it temporal ./ttemporal operator namespace create --namespace custom-namespace
```

*PS: apenas Workers no mesmo namespace podem se comunicar*

---

