# Microservice - Stack

Este compose contém imagens das principais ferramentas que usamos.

Na primeira vez que for utilizar esse pacote use o comando **docker-compose up --build**
Depois, apenas **docker-compose up**

### Eureka - Service Registry

	É uma instância do Eureka, uma solução para registrar microserviços desenvolvida pela Netflix e incorporada ao ecossistema spring, neste serviço vão ser registrados os microserviços que serão desenvolvidos e testados por nós, para acessar e verificar se o microserviço que criou está registrado acesse a URL **localhost:8761**
	
	A documentação se encontra no site *https://cloud.spring.io/spring-cloud-static/spring-cloud-netflix/2.1.2.RELEASE/single/spring-cloud-netflix.html#spring-cloud-eureka-server*

### MongoDB

	Para acessar e configurar no seu projeto a URL deste serviço é **localhost:27017**
	
	Site oficial: *https://www.mongodb.com/*
	
### NoSqlClient
	
	Esse serviço é um gerenciador do mongo, tal como Mongo Compass e Robo Mongo, para usar acesse a URL **localhost:3000**
	Quando acessá-lo configure a conexão com o MongoDB do item anterior.
	
	Incluí este serviço para facilitar a sua configuração de ambiente, caso prefire utilizar um client de sua preferência, fique à vontade para remover essa imagem do docker-compose.
	
	A documentação dele se encontra em *https://www.nosqlclient.com/docs/*
	
### Redis 
	
	Este é uma estrutura de dados chave-valor com armazenamento em memória usamos majoritariamente como cache mas também pode ser utilizado como message broker tal como o RabbitMQ
	Para acessá-lo use a URL **localhost:6379**
	
	Caso queira saber mais sobre esta ferramenta, este é o site oficial: *https://redis.io/*
	
### RabbitMQ

	Este serviço é um Message Broker que implementa o Protocolo AMQP, para acessá-lo e ver as filas, exchanges e bindings criados acesse a URL **localhost:15672** com o usuário e senha *guest*. 
	
	O site oficial com tutoriais e a documentação: *https://www.rabbitmq.com/*
	
### Castle Mock

	Este serviço utilizamos para criar mocks necessários para nossos testes de integração. Para acessá-lo use a URL **localhost:4000/castlemock** com usuário e senha *admin*
	
	O site com a documentação e casos de uso: *https://castlemock.com/*

### ELK Stack

	Este serviço contém 3 imagens, são elas: ElasticSearch, Logstash e Kibana, o objetivo dessa stack é indexar os logs dos microserviços registrados, a URL para acessar o dashboard do Kibana e visualizar os logs criados é **localhost:5601**, esse é o único serviço que não utilizamos a imagem oficial do fornecedor disponível no docker hub, para entender como utilizar essa imagem e consultar possíveis problemas a documentação se encontra no link **https://elk-docker.readthedocs.io/**
	
	Elasticsearch: *https://www.elastic.co/products/elasticsearch*
	Logstash: *https://www.elastic.co/products/logstash*
	Kibana: *https://www.elastic.co/products/kibana*
	

