The software is written in PHP language, it uses MySQL (or MariaDB) as data storage back-end and has a simple but intuitive user interface.

The latest 3.x version is a complete overhaul of the original software.
It is now based on Bootstrap 3 using Bootswatch themes, and still uses CodeIgniter 3 as framework.
It also has improved functionality and security.
Deployed to a Cloud it's a SaaS (Software as a Service) solution.

Server Requirements
-------------------

* PHP version 5.6 to 7.3 are supported. Please note that PHP needs to have `php-gd`, `php-bcmath`, `php-intl`, `php-openssl`, `php-mbstring` and `php-curl` installed and enabled.

* MySQL 5.5, 5.6 and 5.7 are supported, also MariaDB replacement is supported and apparently offering better performance. However you need to disable `only_full_group_by` option, see issue [#2538](https://github.com/opensourcepos/opensourcepos/issues/2538).

* Apache 2.2 and 2.4 are supported. Also Nginx has been proven to work fine, see [wiki page here](https://github.com/opensourcepos/opensourcepos/wiki/Local-Deployment-using-LEMP).

* Raspberry PI based installations proved to work, see [wiki page here](https://github.com/opensourcepos/opensourcepos/wiki/Installing-on-Raspberry-PI---Orange-PI-(Headless-OSPOS)).

* For Windows based installations please read [the wiki](https://github.com/opensourcepos/opensourcepos/wiki) and also existing closed issues as this topic has been covered well in all the variants and issues.


Local install
-------------

First of all, if you're seeing the message **'system folder missing'** after launching your browser, then that means you have cloned the repository and have not built the project properly.

1. Dowload A regular repository clone will not work unless you are brave enough to build the whole project!
2. Create/locate a new mysql database to install open source point of sale into
3. Execute the file database/database.sql to create the tables needed
4. unzip and upload Open Source Point of Sale files to web server
5. Modify application/config/database.php and modify credentials if needed to connect to your database
6. Modify application/config/config.php encryption key with your own
7. Go to your point of sale install public dir via the browser
8. LOGIN for Administrator
  * username: admin 
  * password: admin
  Login For Casier
  * username: yoga
  * password: yoga 
9. Enjoy
10. Oops an issue? you can ask me as issue.