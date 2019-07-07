# wordpress-nginx-php-mysql

Roles "nginx", "php", "wordpress" and "mysql" were created for the initial website
setup and can be used futher for the experiments with Wordpress.


# wp_content-db_import


Roles "wp_content" and "db_import" were created to restore our site from the
existing backup (wp-content.tar.gz and wordpress.sql).

# jenkins-jenkins-content 


Role "jenkins" was created for Jenkins installation. Role "jenkins_content" configures Jenkins.

Just run:
# vagrant up
to check the results:
# https://server-01    (eShop)
# https://server-01/admin
# http://server-03     (Jenkins)

# Username and password for Wordpress and Jenkins:
admin
admin

# Jenkins job description:

Our test eShop (server-01) uses WooCommerce plugin (WC), which is fully integrated with the WordPress REST API. This allows WC data to be created, read, updated, and deleted using requests in JSON format and using WordPress REST API Authentication methods and standard HTTP verbs which are understood by most HTTP clients. 
To add new products to our eShop we are using a command-line tool cURL and the content of the file update.json where the products we want to add are described.
