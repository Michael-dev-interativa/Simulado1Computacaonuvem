
# SIMULADO 1 - Computação em Nuvem

## Saída do docker ps
```
CONTAINER ID   IMAGE          COMMAND                  CREATED         STATUS         PORTS                                     NAMES
b0fe58c277a8   nginx:alpine   "/docker-entrypoint.…"   3 minutes ago   Up 3 minutes   0.0.0.0:8090->80/tcp, [::]:8090->80/tcp   comunicado
```

## Resposta do curl
```
<!DOCTYPE html><html lang="pt-BR"><head><meta charset="UTF-8"><title>Comunicado interno</title></head><body><h1>Comunicado interno disponível</h1></body></html>
```

## Respostas

1. **Diferença entre nginx:alpine e o contêiner comunicado:** `nginx:alpine` é a imagem, o modelo com o Nginx pronto. `comunicado` é o contêiner em execução criado a partir dessa imagem.

2. **Mapeamento 8090:80:** associa a porta 8090 do ambiente à porta 80, onde o Nginx atende dentro do contêiner.

3. **Saída que comprova a resposta:** a saída do `curl` contendo "Comunicado interno disponível". O `docker ps` mostra só que o contêiner está ativo, não o conteúdo da página.
