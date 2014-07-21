SonataAdminBundle

This is the boilerplate for https://github.com/sonata-project/SonataAdminBundle. The code has been configured and tested.

1. Clone the repo:
    git clone https://github.com/sur3s/SonataAdmin/Bundle

2. Install composer following instructions from http://getcomposer.org/. Then run "php composer.phar install" to install them. (It will download all the vendor files so it might take a while to complete.)

3. Go to the 'Setting up Permissions' section of the official symfony setup page i.e. http://symfony.com/doc/current/book/installation.html and choose the suitable method to change the permission of app/cache and app/logs.

4. Make a copy of parameters.yml.dist and rename it to paramters.yml.

5. Config the database parameter in app/config/parameters.yml as
    database_name: (db_name)
    database_user: (db_username)
    database_password: (db_password)

6. Go to the url: http://localhost/project_name/web/app_dev.php/admin/admin/dashboard
  (change the above url as per need)

7. You get the CRUD panel ready to use. But before you start inserting into the database you should create database by console as:
	app/console doctrine:database:create
	app/console doctrine:schema:create

To learn more about the sonataAdminBundle go through the online documentation of the bundle http://sonata-project.org/bundles/admin.

Also the demo website is available at http://demo.sonata-project.org/admin/dashboard (admin as user and password).