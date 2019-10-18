## Endereço da imagem no dockerhub

https://cloud.docker.com/repository/docker/iurynadin/microservicos

- Para executar, rodas comandos na pasta do projeto:
```
docker-compose up -d --build
```

- Visaulizar acessando: http://0.0.0.0:8000/


## Funcionamento do Continuos Deployment
Link vídeo: https://portal.code.education/lms/#/168/155/94/conteudos?capitulo=647&conteudo=5721

- Quando subir algo para qq branch vai rodar a parte de CI.
- Quando colocar qq coisa no master, vai rodar o processo de CI e CD automaticamente
- Organizar um cloudbuild para a área de desenvolvimento e outro para produção
- Um dockerfile normal e um para producao que roda o comando de COPY p copiar os conteudo que a gente criou p dentro do container.

1.Criar um novo cluster
nome do cluster: cluster-docker-laravel

2.Triggers: 
criar umgatilho que toda vez entrar no master, vai rodar o cloudbuild de produção. 
repositorio github: microservicos (fiquei em dúvida se é esse ou o iurynadin/docker-laravel)

