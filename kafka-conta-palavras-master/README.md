# Contador de Palavras

## Requisitos Técnicos

Java 11 | Docker | Docker Compose

## Execução

(x) Após subir o ambiente do kafka, execute o seguinte comando na raiz do projeto:

```
$ docker-compose up
```

(x) Agora no seu terminal, execute a aplicação em spring boot com o seguinte comando:

```
$ ./mwvn clean spring-boot:run
```

(x) Teste na raiz do projeto executando o comando abaixo:

```
$ docker-compose exec kafka kafka-console-producer --bootstrap-server localhost:9092 --topic entrada
>teste alo alo
>123 testando
>
```

(x) Consulte os resultados na raiz do projeto com o seguinte comando:

```
$ docker-compose exec kafka kafka-console-consumer --bootstrap-server localhost:9092 --topic resultado --from-beginning
```

 Finished!