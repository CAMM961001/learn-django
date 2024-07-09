# Imagen base de python
FROM python:3.10.4-slim-bullseye

# Variables de entorno
ENV PIP_DISABLE_PIP_VERSION_CHECK 1
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Directorio dentro del contenedor
WORKDIR /app

# Instalar dependencias
COPY ./requirements.txt .
RUN pip install -r requirements.txt

# Copiar proyecto
COPY . .