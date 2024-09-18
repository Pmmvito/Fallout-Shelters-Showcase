# Fallout Shelters Showcase

Bem-vindo ao projeto Showcase de Abrigos Fallout! Este repositório contém o código para uma aplicação web que exibe vários abrigos fallout. O projeto utiliza o Tailwind CSS para o estilo.

## Voce pode acessar pelo link:
```
https://pmmvito.github.io/Fallout-Shelters-Showcase/
```

## Começando

Para começar com este projeto, você precisará ter o Node.js instalado. Siga os passos abaixo para configurar o ambiente de desenvolvimento e executar o comando CLI do Tailwind CSS.

## Pré-requisitos

- Node.js (inclui npm)
- Tailwind CSS

## Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/fallout-shelters-showcase.git
```

Acesse o diretório do projeto:

```bash
cd fallout-shelters-showcase
```

Instale o Tailwind CSS:

```bash
npm install -D tailwindcss
```

Crie os arquivos de configuração do Tailwind:

```bash
npx tailwindcss init -p
```

## Configuração

Configure o Tailwind CSS:

Certifique-se de que seu arquivo `tailwind.config.js` inclua os caminhos para os arquivos de template:

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    './src/**/*.html',
    './src/**/*.js',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Configure o PostCSS:

Certifique-se de que seu arquivo `postcss.config.js` inclua:

```js
module.exports = {
  plugins: [
    require('tailwindcss'),
    require('autoprefixer'),
  ],
}
```

## Construindo o CSS

Para construir seu CSS usando o Tailwind CSS, execute o seguinte comando:

```bash
npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --watch
```

- `-i ./src/css/input.css` especifica o arquivo CSS de entrada onde as diretivas do Tailwind CSS estão definidas.
- `-o ./src/css/output.css` especifica o arquivo CSS de saída onde o CSS compilado será salvo.
- `--watch` mantém o comando em execução e recompila o CSS sempre que houver alterações no arquivo de entrada.

## Executando o Projeto

Sirva o projeto:

Você pode usar um servidor de arquivos estáticos como  `Live Server` para servir os arquivos HTML ou usar um servidor HTTP simples.

Se você tiver o `http-server` instalado globalmente, pode executar:

```bash
npx http-server
```

Abra o projeto no seu navegador:

    Navegue até http://localhost:8080 (ou a porta fornecida pelo seu servidor) para ver a aplicação em ação.

    Tailwind CSS pelo framework CSS utilitário.
    Font Awesome pelos ícones usados no projeto.
