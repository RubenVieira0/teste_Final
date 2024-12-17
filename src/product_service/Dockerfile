# Usar uma imagem base do Python
FROM python:3.12-slim

# Definir o diretório de trabalho
WORKDIR /app

# Copiar os arquivos necessários
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

# Expor a porta que o gRPC usará
EXPOSE 50051

# Comando para iniciar o servidor gRPC
CMD ["python", "server.py"]