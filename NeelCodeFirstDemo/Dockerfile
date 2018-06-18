from microsoft/dotnet:latest
copy . app
workdir /app

run dotnet restore
run dotnet build

expose 3000
ENV ASPNETCORE_URLS http://*:3000
ENV ASPNETCORE_ENVIRONMENT docker

ENTRYPOINT dotnet run
