# Dockerfile (Criando imagens docker).🐋   🧑‍💻 

##  Dockerfile Um Dockerfile é um arquivo de texto que contém instruções sobre como criar uma imagem Docker. Essas instruções definem o ambiente, as dependências e os comandos necessários para configurar sua aplicação.

Dockerizando uma Aplicação
Passo a Passo 

Criar o Dockerfile:  crie um arquivo chamado Dockerfile no diretório da sua aplicação.

Estruturar a aplicação: Certifique-se de que sua aplicação (por exemplo, um projeto Docker-1) esteja no mesmo diretório ou ajuste os caminhos de cópia no Dockerfile.

## Construindo a Imagem Docker
Com o Dockerfile pronto, você pode construir a imagem usando o comando:

```bash
docker build -t nome-da-imagem:tag .
```
-t nome-da-imagem:tag: Nomeia a imagem. Por exemplo, meu-app:1.0.

.  Indica que o Dockerfile está no diretório atual.

## Executando o Container
Após a construção da imagem, você pode executar um container baseado nela:

```bash
docker run -p 8080:80 nome-da-imagem:tag
```

-p 8080:80: Mapeia a porta 80 do container para a porta 8080 da sua máquina.

nome-da-imagem:tag: O nome e a tag da imagem que você criou.


 ## Comandos Úteis

Listar Imagens:

```bash
docker images
```
Listar Containers:
```bash
docker ps -a
```
Remover uma Imagem:
```bash
docker rmi nome-da-imagem:tag
```
Remover um Container:
```bash
docker rm nome-do-container
```


![dk1](https://github.com/user-attachments/assets/5e0e709b-9e29-4370-bb5d-1ed66afd7bcf)



![dk2](https://github.com/user-attachments/assets/2a567263-d38a-4bbc-8088-ca444c6bf90f)



