<h1 align="center">Product Catalog API</h1>

## :computer: Projeto

Repositório de uma Web API desenvolvida para fins acadêmicos com o propósito de simular um um catálogo de produtos aplicando conceitos da `Clean Architecture`, o código fonte do projeto foi baseado no curso [Clean Architecture Essencial - ASP .NET Core com C#](https://www.udemy.com/course/clean-architecture-essencial-asp-net-core-com-c/). 

Essa aplicação dispõe de um catálago com funcionalidades para  `inserir`, `buscar`, `atualizar` e `excluir` registros em um relacionamento do tipo `1:N` (um para muitos) onde uma `Categoria` possui vários `Produtos`, mas um `Produto` só pertence a uma  `Categoria`.

Usando o `Entity Framework Core` e os recursos do `Code First Migrations` foram realizadas implementações das entidades em uma base de dados criada com o `SQL Server 2019`, 
foram implementados recursos para `Autenticação` e `Autorização` de usuários na aplicação utilizando o `Identity` e `JWT`.

## :white_check_mark: Decisões Técnicas

Algumas decisões tecnicas foram tomadas durante o processo de desenvolvimento:

- a utilização de um base de dados usando uma imagem no `Docker`, foi necessária essa abordagem porque o projeto foi criado em um ambiente Linux.
- optei em não usar o padrão CQRS para a entidade `Product`, essa decisão foi tomada por se tratar de um projeto simples com um CRUD e sua estrutura atual atende bem a ideia da aplicação.
- o reaproveitamento do `Identity` em conjunto com o `JWT`, foram utilizado alguns recursos de ambas as tecnologias para a implementação de sugurança da API, o instrutor inicialmente tinha realizado a implantação de segurança apenas com o `Identity`, ao criar o projeto relacioado a API resolvi manter a mesma ideia que foi apresentada nas aulas de integrar o `JWT` com o `Identity`.

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

```git clone https://github.com/pauloamjdeveloper/dotnet-product-catalog-api.git```

## :camera: Screenshot

<p align="center"> <img src="https://github.com/pauloamjdeveloper/dotnet-product-catalog-api/blob/master/src/ProductCatalog.WebAPI/assets/images/screenshot.png" /></p>

## Author
:boy: [Paulo Alves](https://github.com/pauloamjdeveloper)
