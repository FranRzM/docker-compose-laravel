# docker-compose-laravel

- [Instala Docker](https://docs.docker.com/), y después clona este repositorio.
- Ejecuta `docker-compose up -d --build`.
- Ejecuta `laravel new app` para instalar laravel dentro de una carpeta llamada app.
- Laravel está instalado y funcionando en [http://localhost:8080](http://localhost:8080)

---

#### Para utilizar composer, npm o artisan sería de la siguiente manera:

- `docker-compose run --rm composer install`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 

Estos comandos se tienen que ejecutar en la carpeta raiz.

---

#### Los contenedores que se crean, y sus respectivos puertos son:

- **nginx** - `:8080`
- **mysql** - `:3306`
- **php** - `:9000`
- **npm**
- **composer**
- **artisan**
