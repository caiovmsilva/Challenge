# Resultado - Desáfio CoorLab

A fim de realizar o Desafio Coorlab proposto, foi necessário um estudo sobre as tecnologias Vue.js e FastAPI.

De início, a implementação se deu de maneira muito lenta por conta da falta de familiaridade com ambas as tecnologias (em especial o vue.js). Um fator que dificultou e tardou o término da minha implementação foi o fato de eu estar com a visão limitada por conta de um período de conjuntivite que coincidiu com o prazo estipulado pelo desafio.

De qualquer forma, a implementação em si correu da seguinte forma:

Dentro do diretório app, foram criados dois outros diretórios principais: desafioVue e src. O primeiro comporta todo a implementação do Front-end, na qual foi utilizada Vue.js como tecnologia principal. Já o segundo guarda a implementação do Back-end usando Python e o arquivo JSON como base de dados.

Sobre a implementação do Front, temos os seguinte arquivos:
### App.vue
- Trata-se do arquivo pincipal, onde há a estilização e template da páquina html que é usada de base para a implementação do desafio.

### main.js
- É o arquivo que cria a aplicação vue usado para a implementação, então nele há os principais imports (tanto do vue quanto do vuestic-ui - framework utilizado para criar alguns elementos da aplicação)

### api.js 
- É o arquivo que recebe as requisições da API e retorna para que sejam utilizadas pelo FRONT

## Components
A fim de facilitar a distribuição e organização da aplicação, foram criados três **components**:

### BookTrip.vue
- É o **component** responsável pela estrutura principal da aplicação. Desse modo, a conexão com a API, a utilização dos outros **components** e toda a estilização principal da implementação do desafio foi feita aqui.

### TripResult.vue
- É o **component** que mostra o resultado da busca pelas melhores alternativas de viagem, sendo assim, utiliza o resultado da requisição da API (considerando o JSON como banco de dados) para montar a exibição dos valores de forma semelhante ao exemplo mostrado como protótipo.

### WarningCard.vue
- É o **component** responsável por indicar que o usuário precisa preencher os campos de destino e data para acessar os resultados da busca.

Sobre a implementação do Back, temos os seguintes aquivos:

### data/data.json
- Arquivo JSON usado como base de dados 

### scripts/main.py
- Arquivo responsável por receber as requisições e retornar o que foi pedido, considerando o local e data desejados. É onde a API realmente está implementada.

### scripts/trips.py
- Arquivo responsável pelo tratamento e consumo do arquivo json como banco de dados para a aplicação.
- É onde toda a lógica para selecionar a melhor viagem está.


Por fim, gostaria de destacar que, apesar de trabalhoso, foi um projeto muito legal de ser feito!