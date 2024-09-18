# Showcase de Abrigos Fallout

Bem-vindo ao projeto Showcase de Abrigos Fallout! Este repositório contém o código para uma aplicação web que exibe vários abrigos fallout. O projeto utiliza o Tailwind CSS para o estilo.

## Começando

Para começar com este projeto, você precisará ter o [Node.js](https://nodejs.org/) instalado. Siga os passos abaixo para configurar o ambiente de desenvolvimento e executar o comando CLI do Tailwind CSS.

### Pré-requisitos

- [Node.js](https://nodejs.org/) (inclui npm)
- [Tailwind CSS](https://tailwindcss.com/docs/installation)

### Instalação

1. **Clone o repositório:**


   git clone https://github.com/seu-usuario/fallout-shelters-showcase.git

    Acesse o diretório do projeto:



cd fallout-shelters-showcase

Instale as dependências:

Se você ainda não instalou o Tailwind CSS, você pode adicioná-lo ao seu projeto executando:


npm install -D tailwindcss

Crie os arquivos de configuração do Tailwind:

Se você ainda não criou tailwind.config.js e postcss.config.js, pode fazê-lo executando:


npx tailwindcss init



npx tailwindcss init postcss

Configure o Tailwind CSS:

Certifique-se de que seus arquivos tailwind.config.js e postcss.config.js estejam corretamente configurados. Seu tailwind.config.js deve incluir os caminhos para os arquivos de template, assim:

javascript

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

E o seu postcss.config.js deve incluir:

javascript

    module.exports = {
      plugins: [
        require('tailwindcss'),
        require('autoprefixer'),
      ],
    }

Construindo o CSS

Para construir seu CSS usando o Tailwind CSS, execute o seguinte comando:


npx tailwindcss -i ./src/css/input.css -o ./src/css/output.css --watch

    -i ./src/css/input.css especifica o arquivo CSS de entrada onde as diretivas do Tailwind CSS estão definidas.
    -o ./src/css/output.css especifica o arquivo CSS de saída onde o CSS compilado será salvo.
    --watch mantém o comando em execução e recompila o CSS sempre que houver alterações no arquivo de entrada.

Executando o Projeto

    Sirva o projeto:

    Você pode usar um servidor de arquivos estáticos como Live Server para servir os arquivos HTML ou usar um servidor HTTP simples.

    Se você tiver o http-server instalado globalmente, pode executar:


    npx http-server


    Abra o projeto no seu navegador:

    Navegue até http://localhost:8080 (ou a porta fornecida pelo seu servidor) para ver a aplicação em ação.

Contribuindo

Contribuições são bem-vindas! Se você quiser contribuir, por favor, faça um fork do repositório e crie um pull request.
Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.
Agradecimentos

    Tailwind CSS pelo framework CSS utilitário.
    Font Awesome pelos ícones usados no projeto.
