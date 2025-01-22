# Dockerfile para Atividade 1

# 1. Use a imagem oficial do nginx com menor tamanho possível
FROM nginx:alpine

# 2. Defina o diretório de trabalho no container
WORKDIR /app

# 3. Copie o arquivo index.html para o diretório de trabalho
COPY index.html /app/

# 4. Defina a variável de ambiente APP_VERSION com o valor "1.0.0"
ENV APP_VERSION=1.0.0

# 5. Instale os aplicativos curl, htop e wget
RUN apk add --no-cache curl htop wget

# 6. Exponha a porta 80 para comunicação TCP
EXPOSE 80

# 7. Garanta que o serviço nginx seja iniciado ao iniciar o container
CMD ["nginx", "-g", "daemon off;"]
