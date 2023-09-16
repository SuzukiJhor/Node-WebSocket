# Node-WebSocket

Uma aplicação simples de sorteio em tempo real utilizando WebSockets.

## Descrição

Esta aplicação consiste em duas partes principais:

1. **Admin**: Uma interface para realizar o sorteio e visualizar a quantidade de participantes conectados.
2. **Cliente**: Uma interface para os usuários se conectarem e participarem do sorteio. Quando o sorteio é realizado, a interface do cliente muda de cor e mostra um código se o usuário ganhar.

## Tecnologias Utilizadas

- **Node.js** para o backend.
- **Express** para servir a aplicação web.
- **WebSocket** para comunicação em tempo real entre o servidor e os clientes.

## Configuração e Instalação

### Pré-requisitos

- Node.js instalado. [Veja como instalar aqui](https://nodejs.org/).

### Passos para configuração

- **Clonar o Repositório**

```
git clone https://github.com/SuzukiJhor/Node-WebSocket.git
cd Node-WebSocket
```

- ### Instalar dependências

```
npm install
```
- ### Iniciar o Servidor

```
npm start
```

## Configuração do WebSocket

Para habilitar a comunicação em tempo real, usamos WebSockets. O servidor server.js cuida de aceitar conexões de clientes e admin. A lógica de sorteio e comunicação de resultados é tratada aqui.

client.js: Cada cliente conecta-se ao servidor usando WebSockets. Eles recebem atualizações em tempo real quando um sorteio é realizado.
admin.js: A interface do administrador se conecta ao servidor como um cliente especial. A partir daqui, o admin pode iniciar um sorteio.


## Estilização e Feedback Visual

O arquivo styles.css fornece a estilização necessária para as páginas do cliente e do admin. Durante e depois de um sorteio, a interface do cliente muda de cor para indicar se ganharam ou perderam. O código de confirmação (para vencedores) é exibido em um estilo que se assemelha a um ticket, com um fundo branco, fonte preta e grossa, e bordas arredondadas.

Feedback Tátil

Se o dispositivo suportar, ele vibrará após o resultado do sorteio ser anunciado, dando um feedback tátil ao usuário.

## Como Executar o Sorteio

Abra a página de administração em http://localhost:3000/admin.
Verifique quantos clientes estão conectados através do contador de participantes.
Clique no botão "Realizar Sorteio" para iniciar o sorteio. Um código de confirmação será gerado.
Todos os clientes receberão o resultado em tempo real. O vencedor verá o código de confirmação em sua tela.

## Apresentação:

⚒️
✖️

<img width="780" alt="image" src="https://github.com/SuzukiJhor/Node-WebSocket/assets/95131108/ea85cf20-c04a-4e62-9671-992744601f86">


<br><br>


![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)


