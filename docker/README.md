# Fazendo build da imagem

```
docker build -t gomex/gog .
```

No lugar de "gomex" utilize seu usuário da nuvem hub.docker.com

# Iniciando a imagem

```
docker run -d -p 8080:8080 -p 9990:9990 gomex/gog
```

Acesse no navegador 127.0.0.1:8080

## OBS

Falta configuração do  módulo de conexão do banco de dados
