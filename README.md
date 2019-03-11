# Getting started
## First run

1. Clone the repository

   ```bash
   git clone --recursive https://github.com/karmrt/laradock_symfony.git
   ```

1. Go to laradock directory

   ```bash
   cd laradock_symfony/laradock
   ```   
1. Run containers

   ```bash
   docker-compose up -d nginx mysql
   ```
1. Install dependencies

   ```bash
   docker-compose exec -u laradock workspace composer intall
   ```
1. Visit http://localhost/

## Running tests

```bash
docker-compose exec -u laradock workspace bin/phpunit
```