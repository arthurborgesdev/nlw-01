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

Aqui o principal é a declaração da constante app que recebe a função express();
`const app = express()`

### web

### mobile
