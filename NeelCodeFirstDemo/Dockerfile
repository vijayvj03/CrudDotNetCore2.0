FROM microsoft/dotnet:latest
COPY . app
WORKDIR /app
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

expose 80
ENV ASPNETCORE_URLS http://*:80
ENV ASPNETCORE_ENVIRONMENT docker