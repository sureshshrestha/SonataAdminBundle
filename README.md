This is a ready to use repository for **SonataAdminBundle** configured in **symfony2.5.1**. This is intended for the Symfony developers who want to run into SonataAdminBundle without any burden in configuring. For more details on installation details please go through the official documentation of [SonataAdminBundle](https://github.com/sonata-project/SonataAdminBundle).

1. Clone the repo:

	it clone https://github.com/sur3s/SonataAdminBundle`

2. Install composer following instructions from [here](http://getcomposer.org/). Then run composer install:
	
	php composer.phar install'

	It will download all the vendor files so it might take a while to complete.)

3. Go to the '*Setting up Permissions*' section of the [official symfony setup page] (http://symfony.com/doc/current/book/installation.html)


	Choose the suitable method to change the permission of *app/cache* and *app/logs*.

4. Make a copy of *parameters.yml.dist* and rename it to *paramters.yml*.

5. Config the database parameter in *app/config/parameters.yml* as

	`database_name: (db_name)`

	`database_user: (db_username)`
    
	`database_password: (db_password)`

6. Go to the url: 
	
	*http://localhost/project_name/web/app_dev.php/admin/admin/dashboard*

	(change the above url as per need)

7. You get the CRUD panel ready to use. But before you start inserting into the database you should create database by console as:

	`pp/console doctrine:database:create`

	`pp/console doctrine:schema:create`

To learn more about the sonataAdminBundle go through the online documentation of the [SonataAdminBundle](http://sonata-project.org/bundles/admin).

Also the demo website that demonstarates the features of the bundle is available [here](http://demo.sonata-project.org/admin/dashboard)
	(**admin** as *user* and **admin** as *password*).
