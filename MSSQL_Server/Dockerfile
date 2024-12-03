# Imatge base
ARG MSSQL_VERSION=2022-latest
FROM mcr.microsoft.com/mssql/server:${MSSQL_VERSION}

# Switch to root to perform privileged actions
USER root

# Configuració de la zona horaria
ENV TZ=Europe/Madrid
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# Switch back to the default mssql user
USER mssql