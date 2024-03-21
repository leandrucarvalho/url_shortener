# Encurtador de URL (Node.js)

Este é um projeto de encurtamento de URL desenvolvido como parte da aula prática gratuita da  [Rocketseat](https://www.rocketseat.com.br/) sobre programação. O objetivo deste projeto é construir um sistema de encurtamento de URL completo, incluindo a capacidade de encurtar URLs, monitorar métricas de cliques nos links e demonstrar habilidades em back-end utilizando Node.js, Fastify, PostgreSQL, Redis, TypeScript e Docker.

## Funcionalidades

- Encurtamento de URLs longas para URLs curtas.
- Redirecionamento de URLs curtas para suas respectivas URLs originais.
- Monitoramento de métricas de cliques nos links encurtados.
- Interface de API para interação com o sistema.

## Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas em seu sistema:

- Node.js
- Docker
- npm ou yarn
- PostgreSQL
- Redis

## Configuração

1. Clone este repositório para o seu ambiente local.
2. Execute `npm install` ou `yarn install` para instalar as dependências do projeto.
3. Crie um arquivo `.env` na raiz do projeto e configure as variáveis de ambiente necessárias. Você pode seguir o exemplo do arquivo `.env.example`.
4. Execute o comando `npm run dev` ou `yarn dev` para iniciar o servidor de desenvolvimento.

Certifique-se de ter o PostgreSQL e o Redis em execução em sua máquina local e configurados corretamente conforme especificado no arquivo `.env`.

## Uso

Após a configuração e inicialização do servidor, você pode começar a interagir com a API para encurtar URLs e visualizar métricas de cliques.

### Encurtar uma URL

Envie uma solicitação HTTP POST para `/shorten` com o seguinte corpo JSON:

```json
{
  "url": "URL_LONGA_A_SER_ENCURTADA"
}
```

A resposta conterá a URL encurtada.

### Redirecionar uma URL

Acesse a URL encurtada fornecida pelo sistema para ser redirecionado para a URL original.

### Visualizar métricas de cliques

Envie uma solicitação HTTP GET para `/metrics/:shortCode`, onde `:shortCode` é o código da URL encurtada. Isso retornará as métricas de cliques para essa URL específica.

## Contribuição

Contribuições são bem-vindas! Se você quiser melhorar este projeto, sinta-se à vontade para abrir um problema ou enviar uma solicitação de pull request.

## Licença

Este projeto é licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).
