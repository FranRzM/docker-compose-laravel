# docker-compose-laravel

- [Instala Docker](https://docs.docker.com/), y después clona este repositorio.

- Ejecuta `laravel new app` para instalar laravel dentro de una carpeta llamada app.

- Modifica el archivo `./app/.env` de laravel con los siguientes datos para la BBDD:
    - DB_CONNECTION=mysql
    - DB_HOST=mysql
    - DB_PORT=3306
    - DB_DATABASE=YOUR_DATABASE_NAME
    - DB_USERNAME=YOUR_DATABASE_USER
    - DB_PASSWORD=YOUR_DATABASE_PASSWORD

- Modifica el archivo `docker-compose.yml` con los siguientes datos para la BBDD:
    - DB_CONNECTION=mysql
    - DB_HOST=mysql
    - DB_PORT=3306
    - DB_DATABASE=YOUR_DATABASE_NAME
    - DB_USERNAME=YOUR_DATABASE_USER
    - DB_PASSWORD=YOUR_DATABASE_PASSWORD

- Ejecuta `docker-compose up -d --build`.

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
