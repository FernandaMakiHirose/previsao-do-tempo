# Projeto para consultar a previsão do tempo via API
Desenvolvi um aplicativo de previsão do tempo utilizando Angular como tecnologia front-end cosumindo uma API externa, utilizando o estado da aplicação com práticas avançadas.

![screencapture-localhost-4200-2021-08-22-17_12_03](https://user-images.githubusercontent.com/72028645/130368733-bb9a02fe-e1a5-485a-bdad-24b34c5002e2.png)

## Requisitos
- Node.js e Angular instalados.
- Editor de texto / IDE.
- API key do OpenWeather.

## Como obter uma API key do OpenWeather?
Faça login no site OpenWeather e vá em [API keys](https://home.openweathermap.org/api_keys).

## Depois de clonar o projeto
No projeto:
>npm install

Executar o projeto:
>ng serve

Abra o projeto no navegador:
>http://localhost:4200/

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
`home.effects.ts`: Reagem a uma action de forma assíncrona, baseados em Observables, é possível fazer uma request HTTP. <br>
`bookmarks`: Apresenta as configurações das cidades em favorito. <br>
