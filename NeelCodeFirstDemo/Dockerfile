from microsoft/dotnet:latest
copy . app
workdir /app

run dotnet restore
run dotnet build

expose 8000
ENV ASPNETCORE_URLS http://*:8000
ENV ASPNETCORE_ENVIRONMENT docker

ENTRYPOINT dotnet run
