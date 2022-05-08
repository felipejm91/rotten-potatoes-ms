# Projeto Rotten Tomatoes Microsserviços

## Estrutura do projeto
Esse projeto é baseado em uma aquitetura de Microsserviços e depende de outros 2 projetos pra funcionar

- [Serviço de Filmes](https://github.com/kubedev/movie)
- [Serviço de Review](https://github.com/kubedev/review)

Segue abaixo o diagrama:

![Diagrama da solução](./img/diagrama.png)

## Configuração

MOVIE_SERVICE_URI => URL de acesso ao serviço de listagem de filmes

REVIEW_SERVICE_URI => URL de acesso ao serviço de listagem de reviews

Exemplo:

MOVIE_SERVICE_URI: http://movies:8181

REVIEW_SERVICE_URI: http://review:8282


-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=

CRIAÇÃO DO DOCKERFILE E CRIAÇÃO DO AMBIENTE

Foi criado o documento "Dockerfile" para criação da imagem da aplicação e posterior utilização no ambiente da aplicação rotten-potatoes-ms

O arquivo docker-compose.yaml documenta toda a criação do ambiente da aplicação, utilizando as imagens da aplicação "movies", "review", mongodb e postgresql

O acesso é relaizado através do endereço http://localhost:8080