# Nodejs | Docker | Container.

Simples projeto que mostra o uso de Docker em um projeto Nodejs.

## Para usar:

Fazer o clone deste repositório:

Você precisa ter o [Docker](https://www.docker.com/) instalado em sua máquina.

No terminal acesse o diretório `src` do projeto.

1 - Criar a imagem docker do projeto.
<br> ps: Por boas práticas o nome da sua imagem deve seguir o padrão `namespace/repositorio:versao`, <br>ex: imagemdocker/api-conversor:v1
 - Execute o comando `docker image build -t imagemdocker/conversao-temperatura:v1 .`
 - para consultar se sua imagem realmente foir criada use o comando `docker image ls`

2 - Executar o container com a imagem criada anteriormente.
 - Execute o comando `docker container run -d -p 8080:8080 imagemdocker/conversao-temperatura:v1`
 
## Pronto.
Se tudo deu certo ate aqui, você pode acessar a url http://localhost:8080/ e ver a sua aplicação funcionando.
