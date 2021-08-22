# Projeto para consultar a previsão do tempo via API
Desenvolvi um aplicativo de previsão do tempo utilizando Angular como tecnologia front-end cosumindo uma API externa, utilizando o estado da aplicação com práticas avançadas.

## Pré-requisitos
- Node.js e Angular instalados.
- Editor de texto / IDE.
- API key do OpenWeather.

## Como obter uma API key do OpenWeather?
Faça login no site OpenWeather e vá em [API keys](https://home.openweathermap.org/api_keys).

## Depois de clonar o projeto
No projeto:
>npm install

## Comandos
Gerar um módulo:
>ng g m pasta/módulo

Criar um componente com o tipo `Page`:
>ng g c pasta/módulo --type page

Criar um serviço sem arquivo de teste:
>ng g s pasta/serviço --skipTests true

## Instalações feitas
NgRx:
>ng add @ngrx/store

Store Devtools (faz o binding):
>ng add @ngrx/store-devtools

Instale no Chrome a extensão: `Redux DevTools` (é possível ver o estado da aplicação)

Effects:
>ng add @ngrx/effects

## Entendendo o código
`environment.ts`: Localiza-se a API key. <br>
`environment.prod.ts`: Localiza-se a API key. <br>
`tslint.json`: Da linha 16 até a 20 definição do sufixo, os componentes vão ter o sufixo `Page`. <br>
`app-routing.module.ts`: Definição das rotas. <br>
`home.page.ts`: Faz o Data Binding (Define como dados em diferentes formatos são mapeados) do conteúdo da `home.page.html`. <br>
`home.page.html`: Apresenta 2 formulários. <br>
`app.module.ts`: Na linha 30 inicializou o json e no `home.module.ts` linha 21 passa a função do reducer. <br>
`home.reducer.ts`: Cria o reducer. <br>
`home.actions.ts`: Despachamento das actions da `home.page.ts`, quando pesquisar por uma cidade, uma action será realizada e o reducer vai lidar com ela, a action vai adicionar o nome da cidade (modifica a store) e como deu subscribe na store o título acima do formulário de pesquisa vai atualizar com o nome da cidade pesquisada.

## Sobre a Autora
Oi, eu sou a Fernanda! Estou aqui para contribuir com meu conhecimento e espero poder ajudar no desenvolvimento profissional de cada um de vocês.

[![Linkedin Badge](https://img.shields.io/badge/-Fernanda_Maki_Hirose-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)](https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)  [![Gmail Badge](https://img.shields.io/badge/-femahi2020@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:femahi2020@gmail.com)](mailto:femahi2020@gmail.com)

