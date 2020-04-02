FROM mcr.microsoft.com/dotnet/core/sdk:3.1

WORKDIR /src

COPY . .

# RUN dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL --version 3.1
# RUN dotnet add package NpgSql.EntityFrameworkCore.PostgreSQL.Design
# RUN dotnet add package Microsoft.EntityFrameworkCore.Design
# RUN dotnet add package Microsoft.EntityFrameworkCore.Tools
# RUN dotnet add package Microsoft.EntityFrameworkCore.Tools.DotNet

# RUN dotnet build
# RUN dotnet restore

# RUN dotnet tool install --global dotnet-ef --version 3.1.3
# RUN export PATH="$PATH:/root/.dotnet/tools"

# RUN dotnet build

# RUN dotnet ef migrations add initial
# RUN dotnet ef database update

RUN dotnet publish -c Release -o publish
CMD ["dotnet", "./publish/ContosoPets.Api.dll"]



