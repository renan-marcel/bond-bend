FROM mcr.microsoft.com/dotnet/aspnet:9.0
USER $APP_UID

COPY . /app

WORKDIR /app

ENV DOTNET_SYSTEM_GLOBALIZATION_INVARIANT=false \
    DOTNET_RUNNING_IN_CONTAINER=true

ENTRYPOINT ["dotnet", "BondBend.Aspire.Web.dll"]