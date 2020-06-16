# 🚀 Desafio 01 🚀
Essa foi a primeira tarefa com código, passada no bootcamp GoStack 12. A proposta é simples, mas poderosa: criar uma api funcional para gerenciar repositórios fake, no github, utilizando um CRUD (CREATE READ UPDATE DELETE), armazenando os dados em varáveis, na memória. Também é possível dar likes nos repositórios salvos.

## Conceitos importantes 🤓
### API REST
É a interface que permite comunicar o seu sistema com outras aplicações, por meio do modelo requisição e reposta. Porém, diferente o modelo full mvc, a resposta obtida não é uma página html, somente os dados relvantes para a página criada no front-end.

### Métodos HTTP
É o tipo de requisição que se faz a uma rota. Os principais, são:

* GET - Lista registros

* CREATE - Cria novos registros

* UPDATE - Atualiza registros existentes

* DELETE - Deleta registros

### Parâmetros da Requisição
São dados complementares ao método http. Temos:

* Route params - selecionar registros específicos - na url: '/:parametro'

* Query Params - filtrar resultados de uma busca - na url: '?chave=valor'

### Middlewares
São interceptadores de requisição, que podem bloqueá-la, ou manipular seus dados.

Um pequeno exemplo:

```javascript
  function logRequestParams(request, response, next) {
    const params = request.params;

    console.log(params);

    // caso o next não seja execultado, a requisição não é passada adiante ...
    return next();
  }

  app.use('/users/:id', logRequestParams);
```

### Esse conhecimento te ajudou? 😍
*Avalie o repositório com uma ⭐, para que mais devs possam vê-lo!*

***

Feito com 💜 por [Lucas dos Prazeres](https://www.linkedin.com/in/lucas-prazeres/)