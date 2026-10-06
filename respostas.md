# Respostas · Avaliação Prática de Docker · Cooperativa AgroVale (Turma A)

Nome:
Matrícula:
Usuário do GitHub:
Usuário do Docker Hub:

Responda com as suas palavras e com o que aconteceu na SUA máquina. Resposta curta e certa vale mais
do que texto longo copiado. Resposta que contradiz o seu próprio Dockerfile ou compose vale zero.

## Parte 1 · Dockerfile do portal

1. Qual imagem base você usou e qual o tamanho final da imagem do portal (saída de `docker images`)?
   A imagem base foi "nginx:1.27-alpine" e o tamanho final da imagem gabriellecascardi/agrovale-portal é 73.6MB.

2. Em qual pasta do container o Nginx procura os arquivos do site? Mostre o comando que você usou para conferir que o `index.html` está lá dentro.
   Procura em /usr/share/nginx/html (o que foi determinado no COPY do Dockerfile) e o comando para conferência foi "docker exec teste-portal ls /usr/share/nginx/html".

## Parte 2 · Docker Hub

3. Nome completo da imagem publicada e link público do repositório no Docker Hub.
   O nome da imagem é "agrivale-portal:1.0-26128308" e o link do repositório é "https://hub.docker.com/r/gabriellecascardi/agrovale-portal/tags".

4. Por que o `docker login` foi feito com um token de acesso e não com a senha da conta?
   O token normalmente é utilizado para evitar de expor a senha da conta, então acaba sendo mais uma ação de segurança.

## Parte 3 · Página de manutenção

5. Preencha uma linha por defeito encontrado. Defeito inexistente listado aqui desconta pontos.

| # | Instrução | O que estava errado | O que você viu acontecer | Como corrigiu |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

6. Qual a diferença entre `-p 7042:80` e `-p 80:7042` no `docker run`? Qual dos dois números é a porta do container?

## Parte 4 · docker-compose.yml

7. No serviço `blog`, por que `WORDPRESS_DB_HOST` recebe `db` e não `localhost`?

8. Por que o serviço `db` não publica a porta 3306? Se precisar consultar o banco, como faz sem publicar
   a porta? Mostre o comando.

## Parte 5 · Persistência

9. Quais comandos você usou para derrubar e subir a stack? Qual comando teria apagado o post que você criou,
   e por quê?

10. Código de conclusão impresso pelo verificador:

```
(cole aqui)
```
