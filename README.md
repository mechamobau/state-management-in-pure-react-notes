# Gerenciamento de Estados em React puro

Este repositório contém notas pessoais do curso [State Management in Pure React v2](https://frontendmasters.com/courses/pure-react-state/).

[Slides apresentados: 1 - 8](https://speakerdeck.com/stevekinney/react-state?slide=1)

O curso é apresentado pelo Steve Kinney, _Principal Front Engineer_ da [Twilio](https://twilio.com). Ele tem o foco de apresentar uma visão de gerenciamento de estado no ponto de vista de uma arquitetura Frontend pura utilizando React, sendo ela não mais uma aplicação "de brinquedo" (_toy application_ como ele chama). Os tópicos apresentados no decorrer do curso tem como foco os seguintes itens:

- Pensar profundamente sobre como "estado" significa em uma aplicação React. Definindo e implementando a manipulação de informações e como são apresentadas nas interfaces, assim como os _trade offs_ de tais implementações.
- Aprender um pouco mais sobre como `this.setState` funciona, indo um pouco mais a fundo no funcionamento do estado em componentes de classe.
- Como componentes de classe e hooks se diferem. E principalmente, sendo a Hooks API relativamente nova, como ela se difere no sentido de implementação para migração de componentes classes em componentes funcionais.
- Explorar APIs para resolver `prop-drilling`, problema este que pode ocorrer na má utilização de estado compartilhado.
- Usar reducers para gerenciamento de estado avançado, auxiliando na melhor manipulação do estado das interfaces.
- Escrever os próprios hooks customizados para gerenciamento de estado.
- Armazenar estado no Local Storage.
- Armazenar estado em URLs através de query parameters.
- Buscar dados de um servidor e armazenar em um estado.

De maneira geral, o React possui uma única função:

> O principal trabalho do React é traduzir o estado de sua aplicação em nós do DOM

E como podemos definir o "estado" de nossas aplicações? Isto é visto no próximo item [Tipos de Estado](01/state-types.md)
