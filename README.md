<p align="center">
    <a href="https://github.com/yiisoft" target="_blank">
        <img src="https://avatars0.githubusercontent.com/u/993323" height="100px">
    </a>
    <h1 align="center">Yii 2 Project Desafio</h1>
    <br>
</p>

DIRECTORY STRUCTURE
-------------------

      assets/             contains assets definition
      commands/           contains console commands (controllers)
      config/             contains application configurations
      controllers/        contains Web controller classes
      mail/               contains view files for e-mails
      models/             contains model classes
      runtime/            contains files generated during runtime
      tests/              contains various tests for the basic application
      vendor/             contains dependent 3rd-party packages
      views/              contains view files for the Web application
      web/                contains the entry script and Web resources



REQUIREMENTS
------------

O requisito mínimo para este modelo de projeto é que o seu servidor Web suporte php 5.4.0.


INSTALLATION
------------

### Instalando atraves do arquivo

Crie uma pasta "desafio" em seu computador 

Extraia o projeto baixado para o diretorio que você criou anteriormente


CONFIGURATION
-------------

Configure a chave de validação do cookie no arquivo `config / web.php` para alguma chave secreta aleatória:
```php
'request' => [
    // !!! insira uma chave secreta no seguinte campo(se estiver vazia) - isso é requerido pela validação do cookie
    'cookieValidationKey' => '<secret random string goes here>',
],
```

### Database

Crie um banco de dados chamado desafio.

Edite o arquivo `config/db.php` para configurar seu banco de dados real, exemplo com um banco Mysql:

```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=desafio',
    'username' => 'root',
    'password' => '',
    'charset' => 'utf8',
];
```

Na raiz do projeto, rode o comando 'yii migrate', para criar as tabelas do banco de dados


TESTING
-------

Na raiz do projeto rode o comando 'yii serve' para rodar o servidor web.

Acesse 'http://localhost:8080/' e pronto, seu projeto está rodando localmente.

