FROM microsoft/dotnet:sdk AS build-env
WORKDIR /integration

COPY integration.csproj .
RUN dotnet restore

COPY . . 
ENTRYPOINT [ "dotnet","test" ] 