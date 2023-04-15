FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build
WORKDIR /source
COPY . .
RUN dotnet restore "./ConversaoPeso.Web/ConversaoPeso.Web.csproj" --disable-parallel
RUN dotnet publish "./ConversaoPeso.Web/ConversaoPeso.Web.csproj" -c release -o /app --no-restore

FROM mcr.microsoft.com/dotnet/aspnet:6.0
WORKDIR /app
COPY --from=build /app ./

EXPOSE 80

ENTRYPOINT ["dotnet", "ConversaoPeso.Web.dll"]

