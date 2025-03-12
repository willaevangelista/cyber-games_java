<div align='center', id='topo'/>

# Projeto CyberGames
## Sistema de Loja de Games

</div>

![CyberGames Banner](https://raw.githubusercontent.com/username/cybergames/main/src/main/resources/img/cybergames.png)

O projeto **CyberGames** é uma aplicação backend desenvolvida com o **Spring Framework**. O principal objetivo deste sistema é criar uma **API CRUD** para gerenciar produtos de uma loja de games, organizados por categorias. A aplicação segue boas práticas de desenvolvimento, utilizando uma arquitetura em camadas (*Model, Repository, Controller*) e relacionamento **One to Many** entre **Produto** e **Categoria**.

******

<div align='center'/>

  ![Java](https://a11ybadges.com/badge?logo=java)
  ![Spring](https://a11ybadges.com/badge?logo=spring)
  ![MySQL](https://a11ybadges.com/badge?logo=mysql)
  ![Insomnia](https://a11ybadges.com/badge?logo=insomnia)
</div>


******

## 📖 Tabela de Conteúdo
- [💡 Conhecimentos Mobilizados](#conhecimentosMobilizados)
- [🏗️ Estrutura do Projeto](#estruturaDoProjeto)
- [📂 Código Desenvolvido](#codigoDesenvolvido)
- [🛠️ Tecnologias Utilizadas](#tecnologiasUtilizadas)

---

<div id='conhecimentosMobilizados'/> 

## 💡 Conhecimentos Mobilizados

- **Spring Framework**: Utilização do **Spring Boot** para a construção de **APIs RESTful**, utilizando boas práticas de desenvolvimento e design de APIs.
- **JPA e Hibernate**: Mapeamento **objeto-relacional** para interação com o banco de dados **MySQL**.
- **Padrões de Projeto**: Implementação da **arquitetura em camadas** (*Model, Repository, Controller*) e relacionamento **One to Many** entre as classes **Categoria** e **Produto**.
- **Banco de Dados**: Criação e configuração do banco de dados **MySQL** com uso de **Spring Data JPA** para persistência dos dados.
- **RESTful API**: Desenvolvimento de endpoints para manipulação de **Produtos** e **Categorias**, permitindo operações **CRUD**.

---

<div id='estruturaDoProjeto'/> 

## 🏗️ Estrutura do Projeto
```
cybergames/
├── controller/
│   ├── ProdutoController.java
│   └── CategoriaController.java
├── model/
│   ├── Produto.java
│   └── Categoria.java
├── repository/
│   ├── ProdutoRepository.java
│   └── CategoriaRepository.java
├── resources/
│   └── application.properties
└── CyberGamesApplication.java
```
<div id='codigoDesenvolvido'/> 

## 📂 Código Desenvolvido

Aqui estão os detalhes principais do código:

- **`ProdutoController`**: Controlador responsável pela manipulação dos produtos. Implementa métodos como `getAll()`, `getById()`, `create()`, `update()` e `delete()`.  
- **`CategoriaController`**: Controlador responsável pela manipulação das categorias. Implementa métodos como `getAll()`, `getById()`, `create()`, `update()` e `delete()`.
- **`Produto`**: Modelo que representa a entidade de um produto no banco de dados. Inclui atributos como `id`, `nome`, `descricao`, `preco`, `categoria`, entre outros.  
- **`Categoria`**: Modelo que representa a categoria de um produto, incluindo atributos como `id`, `nome` e o relacionamento com os produtos.
- **`ProdutoRepository`**: Interface que estende `JpaRepository`, permitindo a comunicação com o banco de dados **MySQL** para persistir e consultar produtos.
- **`CategoriaRepository`**: Interface que estende `JpaRepository`, permitindo a comunicação com o banco de dados **MySQL** para persistir e consultar categorias.
- **`application.properties`**: Arquivo de configuração que define a conexão com o banco de dados **MySQL**, incluindo o nome do banco (`db_cybergames`) e outras propriedades do **Spring**.
- **`CyberGamesApplication`**: Classe principal que inicializa a aplicação **Spring Boot**.

---

<div id='tecnologiasUtilizadas'/> 

## 🛠️ Tecnologias Utilizadas

- **Linguagem**: Java  
- **Framework**: Spring Boot  
- **Banco de Dados**: MySQL  
- **JPA/Hibernate**: Para persistência de dados  
- **IDE utilizada**: Spring Tools Suite (STS)
- **Ferramenta de Testes**: Insomnia

<div align='right'>
  
  [Voltar ao topo ⬆️](#topo)

</div>
