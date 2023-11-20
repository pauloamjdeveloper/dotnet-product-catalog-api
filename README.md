<h1 align="center">Product Catalog API</h1>

<p align="center">
  <a href="https://learn.microsoft.com/pt-br/dotnet/"><img alt="DotNet 6" src="https://img.shields.io/badge/.NET-5C2D91?logo=.net&logoColor=white&style=for-the-badge" /></a>
  <a href="https://learn.microsoft.com/pt-br/dotnet/csharp/programming-guide/"><img alt="C#" src="https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white&style=for-the-badge" /></a>
  <a href="https://www.microsoft.com/pt-br/sql-server/sql-server-downloads"><img alt="SQL Server" src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" /></a>
</p>

## :computer: Projeto

Repositório de uma Web API desenvolvida para fins acadêmicos com o propósito de simular um um catálogo de produtos aplicando conceitos da `Clean Architecture`, o código fonte do projeto foi baseado no curso [Clean Architecture Essencial - ASP .NET Core com C#](https://www.udemy.com/course/clean-architecture-essencial-asp-net-core-com-c/). 

Foi desenvolvido um relacionamento do tipo `1:N` (um para muitos) onde uma `Categoria` possui vários `Produtos`, mas um `Produto` só pertence a uma  `Categoria`, usando o `Entity Framework Core` e os recursos do `Code First Migrations` foram realizadas implementações das entidades em uma base de dados criada com o `SQL Server 2019`.

## :camera: Screenshot

<p align="center"> <img src="https://github.com/pauloamjdeveloper/dotnet-product-catalog-api/blob/master/src/ProductCatalog.WebAPI/assets/images/screenshot.png" /></p>

## :wrench: Funcionalidades

Essa aplicação permite ao usuário:

- Utilizar a interace do `Swagger` para acessar os endpoints dos controladores `TokenController`  `CategoryController` e  `ProductController`.
- Gerenciar o catálogo de produtos com as entidades `Produto` e `Categoria` através de operações básicas para `inserir`, `buscar`, `atualizar` e `excluir` registros.
- Executar processos para `Autenticação` e `Autorização` de usuários utilizando o `Identity` e `JWT`.

## :white_check_mark: Decisões Técnicas

Algumas decisões tecnicas foram tomadas durante o processo de desenvolvimento:

- A utilização de um base de dados usando uma imagem no `Docker`, foi necessária essa abordagem porque o projeto foi criado em um ambiente Linux.
- Optei em não usar o padrão CQRS para a entidade `Product`, essa decisão foi tomada por se tratar de um projeto simples com um CRUD e sua estrutura atual atende bem a ideia da aplicação.
- O reaproveitamento do `Identity` em conjunto com o `JWT`, foram utilizado alguns recursos de ambas as tecnologias para a implementação de sugurança da API, o instrutor inicialmente tinha realizado a implantação de segurança apenas com o `Identity`, ao criar o projeto relacioado a API resolvi manter a mesma ideia que foi apresentada nas aulas de integrar o `JWT` com o `Identity`.

## ✔️ Recursos Utilizados

- ``.NET 6``
- ``ASP.NET``
- ``C#``
- ``Entity Framework Core``
- ``Auto Mapper``
- ``ASP .NET Core Identity``
- ``JWT``
- ``Swagger``
- ``SQL Server``
- ``Imagens - Pexels``

## :floppy_disk: Clonar Repositório

```bash
git clone https://github.com/pauloamjdeveloper/dotnet-product-catalog-api.git
```

## :boy: Author

<a href="https://github.com/pauloamjdeveloper"><img src="https://avatars.githubusercontent.com/u/137198048?v=4" width=70></a>
[Paulo Alves](https://github.com/pauloamjdeveloper)

