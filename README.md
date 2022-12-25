README.md

# comandos iniciais
``` bash
mkdir mvc-entity
cd mvc-entity
dotnet new mvc
```
# Comandos git
``` bash
code .gitignore
### gerar código para ignorar os arquivos ( Windows, Linux, Mac, DotnetCore, VisualStudioCode) em https://www.toptal.com/developers/gitignore/
 git init
 git add .
 git commit "primeiro commit"
 git remote add origin git@github.com:RenatoDardengo/Csharp-EntityFramework.git
git branch -M main
git push -u origin main
 ```

 # Componenetes instalados
 ``` bash
 dotnet add package Microsoft.EntityFrameworkCore --version 7.0.1
 dotnet add package Microsoft.EntityFrameworkCore.Tools --version 7.0.1
 dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 7.0.1
 dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 7.0.1
 ```

 # Comandos para migração
  ``` bash
  dotnet tool install --global dotnet-ef
  dotnet ef migrations add CarroAdd
  dotnet ef database update
  ```
  # Instalação do code Generator
   ``` bash
   dotnet tool install -g dotnet-aspenet-codegenerator
   ```

   # Gerando scaffold de Carros
    ``` bash
    dotnet aspnet-codegenerator controller -name CarrosController -m Carro -dc
    DbContexto --relativeFolderPath Controllers

    dotnet aspnet-codegenerator controller -name MarcasController -m Marca -dc
    DbContexto --relativeFolderPath Controllers

    ```




