## Tipos de estado

Existem diversos tipos de estado, é importante saber cada um dos tipos de estado que existem para saber decidir qual abordagem é melhor e qual não é para determinado tipo de estado encontrado.

- **Modelo de dados (_Model data_)**: Os "nomes" dentro da aplicação>
  Os modelos de dados são a camada principal, são realmente os dados núcleo de uma aplicação. Por exemplo em uma _lista de tarefas_, são as **tarefas**. Em um _carrinho de loja virtual_, são os **produtos.** Normalmente se encontram armazenados no servidor, mas este tipo de estado **não é o único!**
- **_View/UI state_**: São os nomes organizados de forma ascendente ou descendente?
  Na camada de dados, na maioria das vezes precisamos nos preocupar com a forma como estes dados são exibidos, se são exibidos e ordenados de determinada forma. Se possuem algum filtro ou apresentação.
  Este tipo de estado da aplicação é o estado da **_View/UI_**, ou seja, o que está sendo exibido para o usuário no momento*.*
- **_Session state_**: O usuário está logado? Quem é o usuário? O usuário pode ver isso?
  É o tipo de estado que define se um usuário está logado ou não, se ele pode visualizar determinado conteúdo ou se ele pode ver parcialmente e etc.
- **Comunicação**: Estamos em um processo de busca (fetching) dos nomes com nosso servidor?
  Conforme fazemos requisições para os [modelos de dados](https://www.notion.so/State-Management-in-Pure-React-Notes-1d18a4e2a99b4f4dbd16f13b543e824b), é importante armazenarmos o estado da requisição (Ela ainda está acontecendo? O que será retornado no final? Está demorando? Teve algum erro?)
- **Localização**: Onde estamos dentro da aplicação? Quais nomes estamos vendo?
  O modelo tradicional da web era baseado em: se você detém um URL, você tem uma localização para um arquivo HTML. Hoje esse modelo mudou, temos um único `index.html` que responde às requisições.
  É armazenada a localização do usuário na aplicação, portanto isto é um tipo diferente de estado.

Genericamente falando, é possível dividir os tipos de estado em dois grandes grupos:

- **Estado do modelo de dados**: Os dados da aplicação. Pode ser o item de uma lista
- **Estado efêmero**: Coisas como o valor de um campo de input que será retornado ao clicar "enter". Isto pode ser a ordem dos itens de uma lista.
