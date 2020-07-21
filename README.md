<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 10: GoRestaurant Web
</h3>

## :rocket: Sobre o desafio

Nesse desafio, foi desenvolvida mais uma aplicação, a GoRestaurant. Foi praticado o que foi aprendindo até agora no React.js junto com TypeScript, praticando o conceito de CRUD (Create, Read, Update, Delete).

Essa é uma aplicação que se conecta a uma fake API, que lida com pratos de refeições, permitindo a criação, exibição, remoção e atualização desses pratos.

Deve-se primeiramente navegar até a pasta criada e executar o comando `yarn` no terminal para instalar todas as dependências.

### Utilizando uma fake API

Antes de tudo, para que existam os dados a serem exibidos em tela, existe um arquivo que será utilizado como fake API, para prover esses dados.

Para isso, está instalada no package.json uma dependência chamada `json-server`, e há um arquivo chamado `server.json` que contém os dados para uma rota `/foods`. Para executar esse servidor basta executar o seguinte comando:

```js
  yarn json-server server.json -p 3333
```

### Layout da aplicação

Essa aplicação possui um layout que você pode seguir para conseguir visualizar o seu funcionamento.

O layout pode ser acessado através da página do Figma, no [seguinte link](https://www.figma.com/file/1lK6AVCPybtWeBLCH8B08N/GoRestaurant?node-id=0%3A1).

Você precisará uma conta (gratuita) no Figma pra inspecionar o layout e obter detalhes de cores, tamanhos, etc.

### Funcionalidades da aplicação

Deve-se verificar os arquivos da pasta `src` e completar onde não possui código, com o código para atingir os objetivos de cada rota.

- **`Listar os pratos de comida da API`**: A página `Dashboard` deve ser capaz de exibir uma listagem, com o campo `title`, `value`, e  `description` e `available` de todos os pratos de comida que estão cadastrados na API.

- **`Adicionar novos pratos de comida na API`**: Na página Dashboard deve-se abrir um modal ao clicar no botão `Novo Prato` no Header. Esse modal deve ser responsável por cadastrar uma nova `food` passando os campos `image`, `name`, `description`, `value`.

- **`Editar pratos de comida da API`**: Na página Dashboard deve-se abrir um modal ao clicar no botão `Editar Prato`. Esse modal deve ser responsável por editar uma `food` passando os campos `image`, `name`, `description`, `value`.

- **`Remover pratos de comida da API`**: Na página Dashboard deve-se remover um prato de comida ao clicar no botão com ícone de lixeira no componente Food.

- **`Alterar disponibilidade dos pratos de comida da API`**: Na página Dashboard deve-se alterar a disponibilidade de um prato de comida ao clicar no switch que é controlado pelo valor de `available`.

### Específicação dos testes

Em cada teste, há uma breve descrição no que a aplicação deve cumprir para que o teste passe.

Para esse desafio, existem os seguintes testes:

* **`should be able to list all the food plates from your api`**: Para que esse teste passe, a aplicação deve permitir que sejam listados, todos os pratos de comidas que são retornados da fake API;

- **`should be able to add a new food plate`**: Para que esse teste passe, deve-se permitir que um prato de comida seja adicionado à API, adicionando-o também à listagem;

- **`should be able to edit a food plate`**: Para que esse teste passe, deve-se permitir que um prato de comida seja editado na API, editando-o também na listagem;

- **`should be able to remove a food plate`**: Para que esse teste passe, deve-se permitir que um prato de comida seja removido da API, removendo-o também da listagem;

- **`should be able to update the availability of a food plate`**: Para que esse teste passe, deve-se permitir que o status do prato de comida seja alterado entre `Disponível` e `Indisponível`.
