# BaltaTeste
Projeto de CRUD feito para o desafio de André Baltieri com código feito através do uso de códigos de comando do dotnet.

[Vídeo do Balta montando o código](https://www.youtube.com/watch?v=fmDYYsSXrKM)

## Comandos passo-a-passo:

Criação do projeto:
```bash
dotnet new razor -o BaltaTest -f net7.0 --auth Individual
```

Adição do Banco de Dados Sqlite
```bash
dotnet add package Microsoft.EntityFrameworkCore.Sqlite
```

Instalando a ferramenta do Entity Framework
```bash
dotnet tool install --global dotnet-ef
```

Adicionando as migrations para fazer as relações com o banco
```bash
dotnet ef migrations add v1 
```

Instalando a ferramenta de geração de código do dotnet
```bash
dotnet tool install -g dotnet-aspnet-codegenerator
```

Adicionando o NuGet Package da ferramenta que instalamos
```bash
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
```

Comando para criar a página Create de estudantes dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Create Create -m Student -dc ApplicationDbContext -sqlite -udl -outDir Pages/Students
```

Comando para criar a página Edit de estudantes dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Edit Edit -m Student -dc ApplicationDbContext -sqlite -udl -outDir Pages/Students
```

Comando para criar a página Delete de estudantes dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Delete Delete -m Student -dc ApplicationDbContext -sqlite -udl -outDir Pages/Students
```

Comando para criar a página Detais de estudantes dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Details Details -m Student -dc ApplicationDbContext -sqlite -udl -outDir Pages/Students
```

Comando para criar a página Index de estudantes dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Index List -m Student -dc ApplicationDbContext -sqlite -udl -outDir Pages/Students
```

Comando para criar a página Create de premiums dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Create Create -m Premium -dc ApplicationDbContext -sqlite -udl -outDir Pages/Premiums
```

Comando para criar a página Edit de premiums dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Edit Edit -m Premium -dc ApplicationDbContext -sqlite -udl -outDir Pages/Premiums
```

Comando para criar a página Delete de premiums dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Delete Delete -m Premium -dc ApplicationDbContext -sqlite -udl -outDir Pages/Premiums
```

Comando para criar a página Detais de premiums dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Details Details -m Premium -dc ApplicationDbContext -sqlite -udl -outDir Pages/Premiums
```

Comando para criar a página Index de premiums dentro do projeto
```bash
dotnet aspnet-codegenerator razorpage Index List -m Premium -dc ApplicationDbContext -sqlite -udl -outDir Pages/Premiums
```