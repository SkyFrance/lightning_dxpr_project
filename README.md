# lightning_dxpr_project


## Authentication

- To access `dxpr/dxpr_builder` packages, you need to subscribe to get access token.

- Configure the access token:

```bash
$ composer config --global bearer.packages.dxpr.com <access_token>
```

## Profile installation

1. `composer clearcache`
2. `composer create-project dxpr/lightning-dxpr-project:1.x-dev <directory_name>`
3. `cd <directory-name>/docroot`
4. `mysql -u root -p -e "drop database tmp;create database tmp;"`
5. `drush site-install lightning_dxpr --db-url=mysql://root@localhost:3306/tmp --account-pass=admin -y -v`
