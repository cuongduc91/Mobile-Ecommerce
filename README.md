# Mobile E-commerce

## Docker

- Download and Install Docker at https://www.docker.com
- Run the .yml file to build the containers as environment
  `docker-compose up`

## db

- As local MySQL database running on port 3310

## DBeaver

- Download and install DBeaver as GUI configuration to the MySQL database
- https://dbeaver.io
- Configuration as MYSQL_USER/MYSQL_PASSWORD in development.env file on port 3320

## Environment file

- Create the development.env file in the main folder.
- Env. Parameters: MYSQL_USER, MYSQL_PASSWORD, MYSQL_ROOT_PASSWORD...

## www

- As the php dockerfile folder running on localhost:8010

## Nodejs

- Download and install npm package via https://nodejs.org/en/
- Initialize the package

```
npm init
```

## SASS

```
npm install -g sass
```

- In case of permission restriction:

```
sudo npm i -g sass
```

## Bootstrap

- Embed the bootstrap links via https://getbootstrap.com

## OWL Carousel

- Embed the links via https://cdnjs.com
- index.js file will serve the function calls of OWL Carousel

## Important!

### Granting privileges to another user

### In terminal:

- For granting user privileges

```
docker exec -it <container name or id>   bash
mysql -u root -p
//loging with root password
GRANT ALL PRIVILEGES ON php_data.* TO '<user name>'@'%' WITH GRANT OPTION;
```
