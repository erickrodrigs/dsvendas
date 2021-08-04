# DSVendas

Aplicação desenvolvida na Semana Spring React do DevSuperior

## Acessar deploy

- [Backend](https://dsvendas-api-erickrodrigs.herokuapp.com)
- [Frontend](https://dsvendas-erickrodrigs.netlify.app/)

## Tecnologias utilizadas

Para desenvolvimento:
- [Spring Boot](https://spring.io/)
- [React.js](https://reactjs.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Docker](https://www.docker.com/)

Para deploy:
- [Heroku](https://www.heroku.com/)
- [Netlify](https://www.netlify.com/)

## Executar aplicação localmente

Para instalar as dependências do frontend localmente:
```bash
docker-compose run --rm web yarn install
```

Para popular o PostgreSQL com os dados fakes:
```bash
docker-compose exec db psql -d dsvendas -U dsvendas -a -q -f data.sql 
```

Para subir os contêineres:
```bash
docker-compose up
```


## Modelo conceitual

<img src="docs/modelo_conceitual.png">
<center>Fonte: <a href="https://raw.githubusercontent.com/devsuperior/bds-assets/main/sds/sds3-mc.png">https://raw.githubusercontent.com/devsuperior/bds-assets/main/sds/sds3-mc.png</a></center>

## Arquitetura do backend

<img src="docs/arquitetura.png">
<center>Fonte: <a href="https://raw.githubusercontent.com/devsuperior/bds-assets/main/sds/camadas.png">https://raw.githubusercontent.com/devsuperior/bds-assets/main/sds/camadas.png</a></center>
