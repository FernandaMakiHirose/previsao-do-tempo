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
