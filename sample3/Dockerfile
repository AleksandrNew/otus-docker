FROM mcr.microsoft.com/dotnet/core/sdk:3.1

WORKDIR /app

ENV ASPNETCORE_URLS=http://*:5000

EXPOSE 5000

COPY src/ /src/

RUN dotnet restore "/src/Otus.Teaching.PromoCodeFactory.sln"

RUN dotnet publish "/src/Otus.Teaching.PromoCodeFactory.WebHost/Otus.Teaching.PromoCodeFactory.WebHost.csproj" -c Release -o /app

CMD dotnet Otus.Teaching.PromoCodeFactory.WebHost.dll
