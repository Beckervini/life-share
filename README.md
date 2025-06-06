Life Share
Aplicação web desenvolvida em ASP.NET Core MVC, focada no compartilhamento de informações entre empresas. O objetivo do projeto é mostrar habilidades práticas em desenvolvimento backend e frontend com .NET, MVC, Entity Framework e boas práticas de programação.

Sobre o projeto
O Life Share permite cadastro e gerenciamento de empresas, login de usuários, e controle de status de empresas. Utiliza Entity Framework para persistência de dados e segue o padrão MVC, com autenticação e proteção de rotas.

Projeto criado como exercício prático para portfólio acadêmico.

Funcionalidades
Cadastro, edição e exclusão de empresas

Autenticação de login

Listagem de empresas com diferentes status

Persistência de dados via Entity Framework

Controle de sessões e exibição de mensagens

Views dinâmicas com Razor

Tecnologias Utilizadas
.NET Core

ASP.NET Core MVC

Entity Framework Core

C#

Razor Pages (Views)

SQL Server (ou SQLite, conforme configuração)

Migrations

TagHelpers personalizados

Estrutura do Projeto
LifeShare/
├── Controllers/
│ ├── EmpresaController.cs
│ ├── HomeController.cs
│ └── LoginController.cs
├── Models/
│ ├── Empresa.cs
│ ├── Login.cs
│ └── Status.cs
├── Persistencia/
│ └── EmpresaContext.cs
├── Migrations/
├── Views/
│ ├── Empresa/
│ ├── Home/
│ ├── Login/
│ └── Shared/
├── appsettings.json
├── Program.cs
├── Startup.cs

Controllers/: lógica das rotas

Models/: entidades de domínio

Views/: páginas renderizadas para o usuário

Persistencia/: contexto de banco

Migrations/: controle de versão do banco de dados

Como rodar o projeto localmente
Clone o repositório
git clone https://github.com/seuusuario/life-share.git
cd life-share/LifeShare

Restaure os pacotes e rode as migrations
dotnet restore
dotnet ef database update

Inicie o projeto
dotnet run

Acesse no navegador: http://localhost:5000 ou porta informada no console.

Obs.: Edite appsettings.json se precisar configurar outro banco de dados.

Autor
Vinicius Becker
Projeto desenvolvido para fins acadêmicos.
