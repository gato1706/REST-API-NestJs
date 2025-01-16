<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

# API REST CRUD de Carros com NestJS

## Este projeto é uma API REST simples para gerenciar carros, desenvolvida com o framework **NestJS**. Foi criada como parte dos meus estudos iniciais no NestJS.

Este projeto foi desenvolvido com base na aula de NestJS do canal Cubos Academy no YouTube. link da aula: https://youtu.be/q8d_w4LPSLE?si=Cv3c3jTjF8gba8ex

## Funcionalidades
- Criar um carro
- Listar todos os carros
- Buscar um carro por ID
- Atualizar informações de um carro
- Deletar um carro

 **Nota:** Este projeto não utiliza banco de dados. Os dados são armazenados em um array na memória, simulando um banco de dados (mock).

## Tecnologias Utilizadas

- [NestJS](https://nestjs.com/)
- Node.js
- TypeScript

## Project setup

```bash
$ yarn install
```

## Compile and run the project

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev


```


## Rotas da API

**GET** <br>
/cars
Retorna todos os carros cadastrados.<br>

**GET By ID** <br>
/cars
Retorna o carro de acordo com o Id.<br>

**POST**  
/cars<br>
Corpo da requisição<br>
 &nbsp;&nbsp;{  
   &nbsp;&nbsp;&nbsp;&nbsp;"brand": "(marca do carro)",  
   &nbsp;&nbsp;&nbsp;&nbsp;"model": "(modelo do carro)",  
   &nbsp;&nbsp;&nbsp;&nbsp;"year": (ano do carro)  
  &nbsp;&nbsp;}<br>

**PATH**  
/cars/id  
Atualiza as informações do carro<br> 
Corpo da requisição<br> 
 &nbsp;&nbsp;{  
   &nbsp;&nbsp;&nbsp;&nbsp;"brand": "( atualize marca do carro)",  
   &nbsp;&nbsp;&nbsp;&nbsp;"model": "(atualize modelo do carro)",  
   &nbsp;&nbsp;&nbsp;&nbsp;"year": (atualize ano do carro)  
  &nbsp;&nbsp;}<br>

**DELETE**  
/cars/id <br>
deleta o carro 



