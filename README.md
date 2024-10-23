# 4. lab. vježba

#### Stvaranje projekta
     dotnet new webapp -n TodoerApp --no-https

#### Stvaranje Git ignore datoteke i repozitorija
     dotnet new gitignore
     git init
     git add .
     git commit -m "Inicijalni commit"

#### Instalacija potrebnih alata
     dotnet tool uninstall --global dotnet-aspnet-codegenerator
     dotnet tool install --global dotnet-aspnet-codegenerator
     dotnet tool uninstall --global dotnet-ef
     dotnet tool install --global dotnet-ef
     
#### Instalacija paketa za scaffolding
     dotnet add package Microsoft.EntityFrameworkCore.Design
     dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
     dotnet add package Microsoft.EntityFrameworkCore.SqlServer
     dotnet add package Microsoft.EntityFrameworkCore.Tools

#### Scaffolding modela
     dotnet aspnet-codegenerator razorpage -m Todo -dc TodoAppDbContext -udl -outDir Pages/Todos --referenceScriptLibraries

#### Izrada migracije
     dotnet ef migrations add AddTodo

#### Ažuriranje baze podataka
     dotnet ef database update

#### Konekcijski string
     Server=sql.vub.zone,14330;Database=korime-aplikacija;User Id=sa;Password=VUBserver2020;TrustServerCertificate=True;Encrypt=False;

# MVC

# API