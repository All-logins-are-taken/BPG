# BFG
# Description
Fully functional page that can add/retrieve/delete/search phone numbers.
The class should prevent to create duplicates.

Used this link to make an array with the country prefix and name https://en.wikipedia.org/wiki/List_of_country_calling_codes
If it can't validate a prefix, then: 07, 02, 03 are Romanian, else german

00 will be converted to +
'-' and space will be replaced with NULL

Insert should return the last insert id, and if duplicate found, it should return the original row id

# How to use
- Written and tested with PHPStorm (I installed PHP 8.0 with php-npm and php-mysql libs, and )
- After install Mariadb 10.6 - https://www.unixmen.com/install-mariadb-arch-linuxmanjaro/ - create DB and User - https://mariadb.com/kb/en/create-user/ (Configured in Storm - https://www.jetbrains.com/help/phpstorm/mariadb.html)
- Inside the settings of the Storm configured interpreter  -  https://www.jetbrains.com/help/phpstorm/configuring-local-interpreter.html ; 
- And configured composer client  - https://www.jetbrains.com/help/phpstorm/using-the-composer-dependency-manager.html; if you do not have previously installed, you can download it  - https://getcomposer.org/download/)
- Then run "composer install"
- copy env.example .env (after it copied you can set your DB preferences)
- To run web server, just go to "cd /src/View" - and execute "php -S localhost:8000" - finally it ready to test; 