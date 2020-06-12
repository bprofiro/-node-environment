<h3 align="center">
  Ambiente de desenvolvimento Node.js
</h3>

<div align="center">
 <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/640px-Node.js_logo.svg.png" width="300px" />
</div>


<div>
  <h2> :rocket: Detalhes sobre o repositório: </h2>
  
  É um ambiente de desenvolvimento Node.js pré-configurado levando o TypeScript como linguagem de desenvolvimento. Ele já vem com as
 configurações de Es-Lint, Prettier e EditorConfig prontas, mas ao clonar o repositório em sua máquina, você pode alterar essas
 configurações você mesmo.
 
  O ambiente já vem com o Express instalado. O Express é um mini-freamework não opinado, portanto, não há uma estrutura fechada de pastas
 pré-configurada, dando liberdade ao desenvolvedor no momento da construção da aplicação.
 
  O mesmo vale para a escolha das ferramentas de padronização de código. O Es-Lint, Prettier e EditorConfig trabalham muito bem com o
 TypeScript e contribuem para a padronização de código dentro de um time de devs e entre os projetos.
  
</div>

<div>
  <h2> 🖥 Utilizando a ambiente: </h2>

  - Para utlizar essa aplicação, você precisará do [Git](https://git-scm.com), [Node.js v10.16][nodejs] ou maior + [Yarn v1.13][yarn] ou maior instalado no seu computador. E então, na sua linha de comando:
  
  ```bash
# Clonar esse repositório
$ git clone https://github.com/bprofiro/node-environment.git

# Entrar na pasta do repositório
$ cd node-environment

# Instalar todas as dependênias
$ yarn install

# Iniciar o servidor:
$ yarn dev:server;
```
</div>

<div>
  <h2> 📃 Configurações no ambiente: </h2>
  
  Ao clonar o repositório e fazer a instalação das dependências, entre no arquivo `package.json` e altere o nome do projeto, colocando o
nome de sua preferência. 

```json
"name": "NOME-DO-PROJETO",
  "version": "1.0.0",
  "main": "index.js",
  "license": "MIT",
  "scripts": {
    "build": "tsc",
    "dev:server": "ts-node-dev --transpileOnly --ignore-watch node_modules src/server.ts"
```

  As alterações no Es-Lint podem ser feitas no arquivo `.eslintrc.json` e as configurações do Prettier no arquivo `prettier.config.js`.
</div>

[nodejs]: https://nodejs.org/
[yarn]: https://yarnpkg.com/

