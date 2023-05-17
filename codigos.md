Códigos Scaffold projeto

Pacotes para instalar no projeto
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 6.0.0
dotnet add package Microsoft.EntityFrameWorkCore.Design -- version 6.0.0
dotnet add package Microsoft.EntityFrameWorkCore.SqlServer -- version 6.0.0
dotnet add package Microsoft.EntityFrameWorkCore.SQLite -- version 6.0.0 

Criacao da Controller
dotnet aspnet-codegenerator controller -name OrdensController -async -api -m Ordem -dc InvestApiContext -outDir Controllers -sqlite

Migrations
dotnet tool install -g dotnet-ef
dotnet ef migrations add InitialCreate 

Criacao do Banco
dotnet ef database update