# FutuereH
Backend -> Drone Feeder.

##
### Contexto:
A empresa FutuereH conseguiu uma nova patente que permitirá a entrega de pacotes com drones. Isso mesmo: o futuro já chegou para FutuereH! Com essa patente registrada, a empresa tem ao todo três meses para iniciar os testes. Sua equipe é responsável por montar o serviço Back-end, que vai fornecer informações aos drones.

Depois de muitas discussões entre os arquitetos e o CTO da empresa, o Back-end foi batizado como Drone Feeder. A Stack escolhida para a criação dele foi a linguagem Java, o banco de dados MySQL, e tudo deve rodar em containers Docker.

A arquitetura da parte do sistema em que o Drone Feeder vai atuar foi entregue à sua equipe pelo CTO e seus arquitetos com o seguinte desenho:

![drone](https://user-images.githubusercontent.com/83831990/174908932-45fc0ee5-f8c4-4b7f-b76c-e4f4816cc520.png)


Confome visto, o Drone Feeder será uma aplicação REST em que um sistema Front-end vai exibir algumas informações dos drones, tais como latitude e longitude, data e horário da entrega ou retirada do pacote. Essas informações serão armazenadas no banco de dados MySQL.

O drone, por sua vez, sincronizará informações com o Drone Feeder sempre que ele tiver uma conexão com a internet. O drone ainda vai informar se a entrega foi efetuada junto a data, horário e vídeo gravado do momento da entrega.

O CTO da FutuereH confia muito na sua equipe e deu liberdade para eventuais melhorias e modificações na arquitetura proposta.
##
### Requisitos técnicos:
- Utilizar Java, MySQL e Docker;
- Gerenciar as dependências com Gradle ou Maven;
- Utilizar framework Spring ou Quarkus para criação do serviço REST.
##
### Funcionalidades:
- Implementar um C.R.U.D. para os drones;
- Implementar um C.R.U.D. para uma entrega associada a um drone;
- Alterar o status da entrega; Extra:
- Implementar três endpoints referentes ao vídeo da entrega sendo realizada:
- Inserir um vídeo
- Listar todos os vídeos
- Baixar (download) de um vídeo específico
