**PT/BR:**

# Projeto Twigoo

## Visão Geral

Bem-vindo ao Twigoo, um projeto de código aberto criado por [Tiago Temporin](https://www.linkedin.com/in/tiago-temporin/). Twigoo é um projeto único que se concentra em construir um serviço personalizável e imutável por meio de arquivos de configuração. Neste README, você encontrará informações essenciais sobre o projeto e seu processo de desenvolvimento.

### Descrição do Projeto

O conceito inicial do Twigoo gira em torno de um usuário interagindo com um serviço, que pode ser uma API ou site. Notavelmente, a implementação é projetada para ser 100% imutável, impulsionada por arquivos de configuração no formato YAML. Esses arquivos de configuração especificam, entre outras coisas, entidades, endpoints, SQL, estruturas de carga e regras de validação, proporcionando um comportamento flexível e configurável para o serviço.

Tiago Temporin compartilhará sua experiência por meio de uma série de vídeos no seu [canal do YouTube](https://www.youtube.com/@AprendaGolang). Embora os vídeos cubram uma variedade de tópicos, nem todos os aspectos do projeto serão ensinados em detalhes. Alguns componentes serão implementados ao vivo, enquanto outros serão explicados pós-desenvolvimento por meio de vídeos gravados.

### [EP.001 - Introdução](https://youtu.be/fAN3LZjXJD4?si=VEilDoevCUQHAXeY)

No primeiro episódio, Tiago introduz o projeto, enfatizando o uso de arquivos de configuração YAML para definir o comportamento do serviço, que pode ser uma API ou site. Os pontos essenciais abordados incluem:

- Entidades
- Endpoints
- SQL
- Estruturas de Carga Útil
- Regras de Validação

O nome do projeto é Twigoo, e Tiago delineia a estrutura e os objetivos do projeto. Algumas implementações de código serão feitas ao vivo, e explicações adicionais serão fornecidas por meio de vídeos gravados.

### [EP.002 - Manifestos Práticos](https://www.youtube.com/watch?v=rFQ0pnxe6Ys)

O segundo episódio é mais prático, mostrando alguns tipos de manifestos inspirados no Kubernetes (k8s). Tiago demonstra um exemplo YAML, fornecendo um esquema para criar a estrutura do banco de dados, um modelo para vincular o esquema a uma entidade de aplicação e um endpoint para especificar detalhes do endpoint. O exemplo YAML se parece com isso:

```yaml
apiVersion: v1alpha
kind: Schema
metadata:
   name: todos
   module: todo
spec:
   columns:
      - name: id
         type: int
         primary: true
      - name: title
        type: string
      - name: description
        type: string
        null: true
      - name: created_at
        type: timestamp
        default: "time.now"
```

Tiago conclui o episódio fornecendo orientações sobre por onde começar, sugerindo que a aplicação deve ler e interpretar os arquivos de manifesto para criar objetos em memória.

## Como Começar

Para começar com o Twigoo, siga estas etapas:

1. Clone o repositório: `git clone https://github.com/twigoo/server`
2. Explore a base de código e os arquivos de configuração.
3. Consulte os vídeos no YouTube para explicações detalhadas e sessões de codificação ao vivo.

Sinta-se à vontade para contribuir com o Twigoo e fazer parte da comunidade de desenvolvedores que moldam o futuro deste emocionante projeto!

---

**EN:**

# Twigoo Project

## Overview

Welcome to Twigoo, an open-source project created by [Tiago Temporin](https://www.linkedin.com/in/tiago-temporin/). Twigoo is a unique project that focuses on building a customizable and immutable service through configuration files. In this README, you'll find essential information about the project and its development process.

### Project Description

The initial concept of Twigoo revolves around a user interacting with a service, which can be an API or a website. Notably, the implementation is designed to be 100% immutable, driven by configuration files in YAML format. These configuration files specify, among other things, entities, endpoints, SQL, payload structures, and validation rules, providing a flexible and configurable behavior for the service.

Tiago Temporin will share his expertise through a series of videos in your [channel on YouTube](https://www.youtube.com/@AprendaGolang). While the videos will cover a range of topics, not every aspect of the project will be taught in detail. Some components will be implemented live, while others will be explained post-development through recorded videos.

### [EP.001 - Introduction](https://youtu.be/fAN3LZjXJD4?si=VEilDoevCUQHAXeY)

In the first episode, Tiago introduces the project, emphasizing the use of YAML configuration files to define the behavior of the service, which can be an API or a website. The essential points covered include:

- Entities
- Endpoints
- SQL
- Payload Structures
- Validation Rules

The project's name is Twigoo, and Tiago outlines the structure and goals of the project. Some code implementations will be done live, and additional explanations will be provided through recorded videos.

### [EP.002 - Practical Manifestos](https://www.youtube.com/watch?v=rFQ0pnxe6Ys)

The second episode is more practical, showing some types of manifests inspired by Kubernetes (k8s). Tiago demonstrates a YAML example, providing a schema to create the database structure, a model to link the schema to an application entity, and an endpoint to specify endpoint details. The YAML example looks like this:

```yaml
apiVersion: v1alpha
kind: Schema
metadata:
   name: todos
   module: todo
spec:
   columns:
      - name: id
         type: int
         primary: true
      - name: title
        type: string
      - name: description
        type: string
        null: true
      - name: created_at
        type: timestamp
        default: "time.now"
```

Tiago concludes the episode by providing guidance on where to start, suggesting that the application should read and interpret the manifest files to create objects in memory.

## Getting Started

To get started with Twigoo, follow these steps:

1. Clone the repository: `git clone https://github.com/twigoo/server`


2. Explore the codebase and configuration files.
3. Check out the YouTube videos for detailed explanations and live coding sessions.

Feel free to contribute to Twigoo and be part of the developer community shaping the future of this exciting project!

---
<p align="center">
  <img src="https://i.pinimg.com/originals/76/70/72/767072baa821ca8414a163220e53bc19.jpg" height="300" alt="Imagem 2">
</p>
