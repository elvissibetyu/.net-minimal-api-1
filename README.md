
# DotNet 6 Minimal Api: Six Min API

## Getting started

### NOTE: This ReadME is for myself since Im still learning DotNet. Sorry if it doesnt help you

#### To generate the app

dotnet new webapi -minimal -n SixMinApi

#### if no ssl run

dotnet dev-certs https --trust

#### to run the project

dotnet run

#### Adding Entiti framework Core Packages

dotnet add package Microsoft.EntityFrameworkCore
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet add package Microsoft.EntityFrameworkCore.SqlServer

#### Adding Auto Mapper --> We want to use some of its dependency injection features

dotnet add package AutoMapper.Extensions.Microsoft.DependencyInjection

#### Initialise user secrets

dotnet user-secrets init

#### Setting a user secret

dotnet user-secrets set "key" "value"

#### To spin up sql server

docker-compose up -d

#### generate RF migrations

dotnet ef migrations add initialmigration
then
dotnet ef database update

#### To install EF Command line tools

dotnet tool install --global dotnet-ef
