# RabbitMQ
Exemplo de Producer and Consumer RabbitMQ

<br>
<div align="center">
  <img src="https://user-images.githubusercontent.com/92545393/233182812-6c55b309-692b-4630-a09c-47d8b0cc7c8e.png" width="300px"/>
</div>
<br>

O RabbitMQ é um dos message broker de código aberto mais populares, sendo utilizado em empresas de todos os tamanhos.
Um message broker é um sistema que permite que diferentes componentes, como aplicações e aplicativos, se comuniquem entre si, trocando informações. Para isso, geralmente utilizam uma estrutura de fila de mensagens, que será a responsável por armazenar e ordenar mensagens enquanto os consumidores (como aplicativos ou aplicações) não as processam.

Voltando ao RabbitMQ: ele é leve, fácil de publicar em diversos ambientes, como localmente, on-premises e em nuvem, suportando diversos protocolos de mensageria. Por exemplo, para testes locais é bem simples de se criar uma instância utilizando Docker.

Como um dos princípios da mensageria, o RabbitMQ possibilita que aplicações se conectem entre si e escalem, de maneira desacoplada.

Principais conceitos:
Vamos agora para os principais conceitos associados ao RabbitMQ:
Fila: estrutura onde as mensagens são armazenadas e consumidas. Tem como principais características, que podem ter valor verdadeiro ou falso:

Durável: a fila segue existindo mesmo que o message broker reinicie;
Auto-Delete: quando a fila chegue a ter apenas um consumidor e ele se desinscreve, a fila é apagada;
Exclusiva: a fila é utilizada por apenas uma conexão, sendo apagada quando essa conexão for encerrada.
Exchange: são os agentes responsáveis por rotear as mensagens para filas, utilizando atributos de cabeçalho, routing keys ou bindings.

Binding: conexão utilizada para configurar uma relação entre uma fila e um exchange.

Routing Key: é um atributo adicionado ao cabeçalho da mensagem, servindo como um “endereço” que o exchange poderá decidir como rotear a mensagem com base nos Bindings definidos.

## ⚙️ Demonstração do projeto em execução

https://user-images.githubusercontent.com/92545393/233692557-a3612cf3-98c6-47a0-a76a-9c7b5ea62bc7.mp4

## 🚀 Começando - Start

A maneira mais fácil de se instalar e iniciar o RabbitMQ é através de um comando utilizando Docker. Extraí do próprio site do RabbitMQ o comando Docker abaixo para se iniciar o RabbitMQ e sua ferramenta de gerenciamento, que conta com uma interface Web.

Consulte https://www.rabbitmq.com/documentation.html para saber mais detalhes.

### 🔧 Instalação

```
# latest RabbitMQ 3.10
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.10-management
```
```
Executar o projeto
Navegar para a rota http://localhost:15672

```

## 🛠️ Construído com as seguintes linguagens e frameworks:

* RabbitMQ
* .NET CORE
* C#



## ✒️ Autor

* **Edilson Madsen**

---
⌨️ com ❤️ por [Edilson Madsen - LinkedLn](https://www.linkedin.com/in/edilsonmadsen/) 😊


