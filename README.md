# nlw-01
Projeto construído durante o Next Level Week #01

Olá pessoal! ;D 

Diferentemente de outros projetos e outros READMEs, vou tratar esse aqui de uma forma diferente. Vou tratar como um diário, em que vou
ir documentando aos poucos tudo que aprendi durante essa semana maravilhosa da Rocketseat! Meu intuito é solidificar ao máximo tudo que
aprendi sobre Node, React e React Native, para que seja útil em consultas futuras para mim ao desenvolver novas aplicações.


## Estrutura de arquivos

### server

Considerado o backend da aplicação. Pasta principal: /src

Na aplicação inteira foi dada a preferência por TS em vez de JS puro, e isso foi muito vantajoso por aproveitar a inteligência da IDE e
também para "tipar" os dados. Vantagens adicionais: (TODO: Ler mais sobre TS com Node e React).

#### src

##### server.ts

Logo durante o desenvolvimento, o Diego concentrou em "fazer funcionar" agrupando as funções em um único arquivo, para depois estruturar
em pastas separadas, então, logo de início não havia uma pré estrutura de pastas como se vê em frameworks como Laravel e Rails, em que 
tudo segue uma estrutura e patterns pré-definidos. Não lembro direito, mas acredito que o "server.ts" sempre foi o arquivo inicial.

(Lembrete: Caso não for reconhecido os tipos pelo VSCode, instalar as dependências correspondentes como desenvolvimento, exemplo:
"@types/express")

server.ts importa path, routes e error (validação de 'celebrate', ver mais tarde).

Aqui o principal é a declaração da constante app que recebe a função express():

`const app = express()`

Depois de definir a constante, faz-se o uso de vários middlewares à função express, do tipo:

app.use("nome do middleware").

Há middleware para CORS, express.json, routes (aqui o express faz uso das rotas que foram definidas em outro arquivo), dos arquivos na pasta /uploads e dos erros (validação de 'celebrate').

Após todos esses middlewares serem chamados (é possível chamar vários outros, pois por definição, express é um framework web de middlewares e rotas - https://expressjs.com/en/guide/using-middleware.html), chama-se a função listen na constante app, passando o número da porta que o app express irá escutar em localhost: 

`app.listen(3333);`

### web

### mobile
