---
title: Curso aTemporal
description: Boas vindas ao nosso cursinho de Temporal.io! Espero que goste.
---

<img src="https://cdn.sanity.io/images/bbnkhnhl/production/325eba542999ccf3b4b41cfeb543c7a8e37a35a9-1460x968.png?w=1200&q=75&fit=clip&auto=format">
# Curso aTemporal


??? tip "Caso prefira ver a apresentação do curso em vídeo"
	Esse aula ainda não está disponível em formato de vídeo, somente em texto ou live!
	<iframe width="560" height="315" src="https://www.youtube.com/embed/8t_nrU5B-Eo?si=KM5JWKQ2UoeZ5DP8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

	[Aula :fontawesome-brands-youtube:](https://www.youtube.com/embed/8t_nrU5B-Eo?si=Kr9zazmhPawFiqUh){ .md-button }


Olá, boas vindas ao nosso curso de Temporal.io!

A nossa intenção neste curso é espalhar a palavra do Temporal.io por aí, na intenção de criar uma comunidade mais forte e que possamos fomentar o uso dele nas empresas do nosso Brasil. Vamos explorar o que é o Temporal.io, como funciona o Temporal Client, ver tudo funcionando direitinho na UI e muito mais. Tudo isso para oferecer uma boa base para quem quer trabalhar com desenvolvimento de workers com Temporal. A ideia desse curso é apresentar os conceitos de forma prática, construindo um projeto do zero e indo até os conceitos mais aprofundados.


## O que é o Temporal?

[Temporal](https://temporal.io/){:target="_blank"} é uma plataforma de orquestração de workflows (fluxos de trabalho) distribuídos e escaláveis. Ele permite que os desenvolvedores criem, executem e gerenciem processos de longa duração, como tarefas que podem envolver múltiplas etapas e interações complexas, sem se preocupar com falhas temporárias ou com a complexidade de gerenciar estados de maneira manual.

## Sobre o curso

Este curso foi desenvolvido para oferecer uma experiência prática no uso do Temporal, uma das ferramentas mais modernas para construções de sistemas resilientes e d longa-duração do mercado. Ao longo do curso, o objetivo é que você obtenha uma compreensão das funcionalidades principais do Temporal e de boas práticas associadas a ele.

Para a construção do projeto, serão utilizadas as versões mais recentes das ferramentas, disponíveis em 2025, como a versão v1.26.2 do Temporal, a versão além da versão v22.14.0 do Node.js (utilizado por mim durante as aulas), e as versões dos packages:

- @temporalio/worker 1.11.7
- @temporalio/common 1.11.7
- @temporalio/workflow 1.11.7
- @temporalio/activity 1.11.7
- @temporalio/client 1.11.7
- @temporalio/testing 1.11.7



Mas vocẽ pode utilizar também o seu SDK da sua liinguagem favorita (Java, .NET, PHP, Golang, Ruby ou Python).

## O que você vai aprender?

Aqui está uma visão geral dos tópicos que abordaremos neste curso:

1. **O que é o Temporal.io e qual o seu propósito**: explicarei como o Temporal facilita a vida de quem quer desenvolver.

2. **Primeiros Passos com Temporal**: Configuraremos o ambiente, mergulharemos na estrutura básica de um worker e faremos alguns workflows simples e activities.

3. **Observalidade e políticas de retentativa**: aprenderemos a ver dados sobre a execução dos nossos workflows e a criar políticas de retentativas, além de testarmos elas na prática.

4. **Comunicação poliglóta**: aprenderemos como fazer nossa aplicação se comunicar com outros Workers de outros microsserviços que podem estar escritos em qualquer um dos SDKs oficiais do Temporal.
   
5. **Temporal Schedulers**: construiremos schedulers que dispararão nossos workflows de forma simples, basicamente um cron-job com esteróides.

6. **Durable executions**: por fim, faremos uma introdução detalhada a execuções de longa duração, workflows que podem rodar infinitamente por anos e como podemos enviar dados, acessar dados do estado do Workflow atual e alterar esse estado para criar novas interações.


## 💰 Esse curso é gratuito?

SIM! Esse curso foi todo desenvolvido [de forma aberta](#licenca){:target="_blank"} e ajuda financeira nenhuma! Caso você sinta vontade de contribuir, você pode me pagar um café por pix (gcsolutions.dev@gmail.com).

## Onde o curso será disponibilizado?

Esse material será disponibilizado de duas formas diferentes:

1. Em livro texto: todo o material está disponível nessa página;

2. Em formato de vídeo (assíncronas): todas as aulas serão disponibilizadas em formato de vídeo em meu canal do [YouTube](https://www.youtube.com/@nice_gustavinho){:target="_blank"} para quem prefere assistir ao ler. (**Vídeos ainda não disponíveis**)

## Pré-requisitos

Para aproveitar ao máximo este curso, é recomendado que você já tenha algum conhecimento mínimo em Programção Orientada a Eventos e entender bastante da linguagem do SDK da sua escolha. Se eu pudesse listar o que considero importante para não se perder, os tópicos importantes são:

- O funcionamento do Docker / docker-compose: como usar ([referência](https://docs.docker.com/compose/){:target="_blank"});
- O conceito de programação funcional e orientação a objeto;
- Classes de dados: o funcionamento básico de class-validator, dataclasses, Hibernate Validator, DataAnnotations enfim, classes que validam dados.
- Desenvolvimento Web e APIs RESTful: não essencial, pois iremos abordar pouco, mas o quanto mais você souber melhor para acompanhar;
- git: não nos aprofundaremos nesse tópico durante o curso, mas usaremos operações básicas de git (como commit e push);

??? info "Caso você manje de inglês"
	Caso você conheça bastante inglês e queira se aprofundar em mais tópicos, o pessoal de Curriculum Developer da própria Temporal Technologies oferecem cursos gratuitos para você ler e testar. Nosso intuito aqui é fazer com que você se sinta melhor acolhido com o diálogo mais intimista de um português quase bem falado, mas você pode ver mais sobre Temporal nos links abaixo.

	- [**Temporal 101**](https://learn.temporal.io/courses/temporal_101/){:target="_blank"}
    - [**Temporal 102**](https://learn.temporal.io/courses/temporal_102/){:target="_blank"}
    - [**Interacting with Workflows**](https://learn.temporal.io/courses/interacting_with_workflows/){:target="_blank"}

## Aulas

# TBD


Após todas as aulas, se você sentir que ainda quer evoluir mais e testar seus conhecimentos, podemos conversar mais no meu [LinkedIsney](https://br.linkedin.com/in/gustavocarneirodev){:target="_blank"}.

### 🐏 Quem vai ministrar essas aulas?

<div class="sbs" markdown>
![Uma fotografia minha, Gustavinho, olhando para a câmera](assets/eu.jpeg){ .shadow}
<div markdown>

Prazer! Eu me chamo Gustavo. Mas as pessoas me chamam de [Gustavinho](https://meuproximo.site/devgustavinho){:target="_blank"}.


Sou um desenvolvedor estudioso e gosto de ajudar as pessoas a se desenvolverem. Toco um projeto pessoal chamado **GC Solutions** há quase 3 anos. Minha intenção é poder criar algo um dia que irá ajudar as pessoas.

Esse projeto é um dos vários projetos que eu toco (ou tento tocar) simultaneamente. Espero que você aprenda bastante e se conecta comigo no [LinkedIn](https://br.linkedin.com/in/gustavocarneirodev){:target="_blank"} para no futuro eu poder recomendar você nas empresas que eu passo!

Sou noivo da [Késsia](https://www.instagram.com/teacherkessialima/), uma professora particular de inglês que a um tempo vem tendo vários alunos da área de Desenvolvimento. Juntos, temos uma gatinha frajola feinha (linda) chamada Kiara Maria. 

🐈‍⬛
</div>
</div>

## :face_with_monocle: Revisão e contribuições

Esse material ainda não foi revisado, mas sinta-se a vontade para criar um pull requests para contribuir!

## 📖 Licença

Todo esse curso foi escrito e produzido por Gustavo Carneiro de Almeida ([@devgustavinho](https://github.com/devgustavinho){:target="_blank"}).

Todo esse material é gratuito e está sob licença Creative Commons [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. O que significa que:

- Você pode copiar e reproduzir esse material em qualquer meio e em qualquer formato;
- Você pode adaptar esse material e construir outros materiais usando esse material.

Pontos de atenção:

- Você precisa dar os devidos créditos a esse material onde for usar ou adaptar;
- Você não pode usar para fins comerciais. Como vender ou usar para obter vantagens comerciais;
- Todo o material derivado desse material deve ser redistribuído com a licença [CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}.

## 🧰 Ferramentas necessárias para acompanhar o curso

1. Um editor de texto ou IDE de sua escolha. Estou usando o [Visual Studio Code](https://code.visualstudio.com/){:target="_blank"} enquanto escrevo as aulas;
2. Um terminal. Todos os exemplos do curso são executados e explicados no terminal. Você pode usar o que se sentir mais a vontade e for compatível com seu sistema operacional;
3. Se for acompanhar em Typescript, ter o `nvm` instalado e trocar a versão para a `v22.14.0` do Node.js. Se for usar outra linguagem, garantir que ela segue as versões recomendadas na documentação do Temporal.

## 🔧 Ferramentas de apoio

Toda essa página foi feita usando as seguintes bibliotecas:

- [MkDocs](https://www.mkdocs.org/){:target="_blank"}: Para geração das páginas estáticas usando Markdown
- [Mkdocs-material](https://squidfunk.github.io/mkdocs-material/){:target="_blank"}: Tema para o MkDocs
- [Mermaid.js](https://mermaid-js.github.io/mermaid/){:target="_blank"}: Construção dos diagramas


### 📁 Repositório
O versionamento de tudo está sendo feito no [repositório do curso Github](https://github.com/devgustavinho/curso-atemporal){:target="_blank"}

### 🚀 Deploy
Os deploys das páginas estáticas geradas pelo MkDocs estão sendo feitos no [Github Pages](https://pages.github.com/){:target="_blank"}

## Conclusão

Neste curso, a intenção é fornecer uma compreensão inicial, mas bem aprofundada, do Temporal.io, utilizando-o para construir diversos cenários reais em que ele pode ser útil. O aprendizado será focado na prática, e cada conceito será acompanhado por exemplos e exercícios relevantes.

Este conteúdo foi pensado para auxiliar na compreensão de como criar microserviços relientes e confiáveis, dando atenção a aspectos importantes como idempotência, observalidade e políticas de retentativas.

Nos vemos na primeira aula. ❤

## F.A.Q.

Perguntas frequentes que me fizeram durante os vídeos:

- Que papel de parede é esse? [É o Gyarados Shine do Wallpaper Engine](https://store.steampowered.com/app/431960/Wallpaper_Engine/?l=portuguese){:target="_blank"}
- Qual o tema no shell? Basiscamente tudo meu é no tema [Dracula](https://draculatheme.com/){:target="_blank"}. O meu Oh-my-zsh! usa o tema [spaceship](https://github.com/spaceship-prompt/spaceship-prompt){:target="_blank"}
- Qual o tema do seu editor? [Dracula](https://draculatheme.com/){:target="_blank"} também
