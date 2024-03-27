# Documentação do Projeto MVC de Agenda de Contatos

## Visão Geral

O Projeto MVC de Agenda de Contatos é uma aplicação web desenvolvida para gerenciar uma lista de contatos, permitindo operações CRUD (Create, Read, Update, Delete). O projeto utiliza o padrão de arquitetura MVC (Model-View-Controller) para organizar e estruturar o código de forma modular e escalável.

## Inicialização
Para executar o projeto, utilize as ferramentas descritas na sessão **Ferramentas**.


## Ferramentas

O projeto foi desenvolvido utilizando as seguintes tecnologias:

- [ASP.NET Core](https://dotnet.microsoft.com/download): Framework para desenvolvimento de aplicativos web utilizando o padrão MVC.
- **C#**: Linguagem de programação utilizada no desenvolvimento do backend.
- [SQL Server](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads): Para gerenciamento e armazenamento do banco de dados.
- **HTML/CSS**: Linguagens de marcação e estilização utilizadas no desenvolvimento das views.
- **Bootstrap**: Framework front-end utilizado para criar interfaces responsivas e estilizadas.


## Links importantes
* [ASP.NET Core Documentation](https://docs.microsoft.com/pt-br/aspnet/core/?view=aspnetcore-6.0) - Documentação oficial do ASP.NET Core.
- [Documentação do C#](https://docs.microsoft.com/pt-br/dotnet/csharp/): Documentação oficial da linguagem de programação C#.
- [Documentação do HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML): Documentação oficial da linguagem de marcação HTML.
- [Documentação do CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS): Documentação oficial da linguagem de estilização CSS.
- [Documentação do Bootstrap](https://getbootstrap.com/docs/5.1/getting-started/introduction/): Documentação oficial do framework Bootstrap.

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- **Controllers**: Contém os controladores MVC responsáveis por processar requisições HTTP e controlar o fluxo de dados.
- **Models**: Contém as classes que representam os modelos de dados utilizados na aplicação.
- **Views**: Contém as views HTML responsáveis por exibir a interface do usuário.

## Modelos de Dados

### Contato

A classe `Contato` representa um contato na agenda. Possui os seguintes atributos:

- **Id**: Identificador único do contato (int).
- **Nome**: Nome do contato (string).
- **Telefone**: Número de telefone do contato (string).
- **Ativo**: Indica se o contato está ativo ou não (bool).

```csharp
public class Contato
{
    public int Id { get; set; }
    public string Nome { get; set; }
    public string Telefone { get; set; }
    public bool Ativo { get; set; }
}
```

## Controladores

### ContatoController

O `ContatoController` é responsável por gerenciar as operações relacionadas aos contatos, incluindo criação, edição, exclusão e visualização.

#### Actions

- **Index**: Retorna a lista de contatos.
- **Criar**: Exibe o formulário para criar um novo contato.
- **criar**: Processa o formulário de criação de um novo contato.
- **Editar**: Exibe o formulário para editar um contato existente.
- **Editar**: Processa o formulário de edição de um contato.
- **Detalhes**: Exibe os detalhes de um contato.
- **Deletar**: Exibe o formulário para confirmar a exclusão de um contato.
- **Deletar**: Processa a exclusão de um contato.

## Views

### Contato

- **Criar.cshtml**: Exibe o formulário para criar um novo contato.
- **Deletar.cshtml**: Exibe os detalhes de um contato e o formulário para confirmar a exclusão.
- **Detalhes.cshtml**: Exibe os detalhes de um contato.
- **Editar.cshtml**: Exibe o formulário para editar um contato existente.
- **Index.cshtml**: Exibe a lista de contatos.

### Home

- **Index.cshtml**: Página inicial da aplicação, com links para a lista de contatos.

## Estilos e Layout

O projeto utiliza o framework Bootstrap para estilização e layout responsivo, proporcionando uma experiência visual agradável e consistente aos usuários.

### Imagens da Aplicação
#### Tela Inicial
![Captura de tela 2024-03-27 182538](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/53732920-9f0e-44de-b66e-fbb4dded9bba)
#### Lista de Contatos
![Captura de tela 2024-03-27 182556](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/2365bc28-4068-44d5-9a21-02a1f4cacd08)
#### Tela de Criar
![Captura de tela 2024-03-27 182616](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/9ebf626a-2a1f-46b1-b589-ba7ccd34908b)
#### Tela de Editar
![Captura de tela 2024-03-27 182638](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/090b1a42-d334-4307-b5b0-a5b983318551)
#### Tela de Detalhes
![Captura de tela 2024-03-27 182652](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/e1c90f02-a83a-467a-bdd4-31e7755580d3)
#### Tela de Deletar
![Captura de tela 2024-03-27 182707](https://github.com/euuhebert/Agenda_Contatos/assets/112333883/0a76578f-e541-4400-9245-358ad7396f73)

## Conclusão

A documentação fornece uma visão geral do projeto, detalhando sua estrutura, tecnologias utilizadas, modelos de dados, controladores, views e estilo. Este projeto é uma aplicação web robusta e funcional para gerenciamento de contatos, oferecendo uma interface intuitiva e eficiente para os usuários.

Este é o resumo da documentação para o Projeto MVC de Agenda de Contatos. Se houver mais alguma informação específica que deseje adicionar ou modificar, por favor, me avise!
