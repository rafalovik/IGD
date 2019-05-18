# Infrastructure Test - API

### Procedimento iniciais 

### Esta aplicação requer os sequintes pacotes instaldos na máquina(instancia). 
---------
* Ruby 2.3 or greater;
* RubyGems and Bundler;
* A PostgreSQL database server;
* A Redis Server;
* Bundler (`gem install bundler`);

### Segue exemplo de como instalar e iniciar a aplicação. 
---------
```
$ git clone git@bitbucket.org:klicksite/infra-test-api.git
$ cd infra-test-api
$ bundle install
$ rake db:setup db:migrate db:seed
$ bundle exec rails s -p 3000 -b '0.0.0.0'
```

### Procedimentos para cria um redis. 
---------
```
https://docs.aws.amazon.com/pt_br/opsworks/latest/userguide/other-services-redis-cluster.html
```

### Variables

*Adicione estas variaveis na sua máquina(instancia) com os valores do banco de dados e Redis.*
----------
View `.api.env-example` file:
```
APP_DATABASE_HOST
APP_DATABASE_PORT
APP_DATABASE_NAME
APP_DATABASE_USER
APP_DATABASE_PASSWORD
APP_REDIS_HOST
APP_REDIS_PORT
```
