Repo forked from [MohammedTsmu's repo](https://github.com/MohammedTsmu/authentication-system-mysql-php-LOGIN-SYSTEM-IN-PHP-AND-MYSQL) to make a more secure version using PDO and anti-SQL -injections techniques.
<br>
Also addind extra-informations like firstname, lastname an role.
<br>
<b>Still in developement</b>

# LOGIN SYSTEM IN PHP AND MYSQL: User Authentication system.

###### VERSION 1.1.0

User authentication in web developement is used to authorized and
restrict users to certain pages in a web appplication.

## REGISTERATION SYSTEM

### DATABASE TABLE IN MYSQL

The database used is MySQL, so you'll need a MySQL database to run create the users table.
Run the `sql.sql` file in MySQL within `login/setup` to create users table.
<br>
*Note that "role" column is still not in use in v1.1.0*

### CONFIGURATION FILE

The PHP script to connect to the database is in `login/config/config.php` directory.
Replace credentials to in `config.php` to match your server credentials.
<br>
**For security reasons, you should not use 'root' accounts. It is is recommended to create a specific user for the login system such as 'system.login'. You can find the query in `login/setup/user.sql`**

### REGISTERATION FORM AND SCRIPT

The `register.php` creates a web form that allows users to register themselves.
The script generates error if form input is empty and username is has been taking already by another user.

## LOGIN SYSTEM

### LOGIN FORM AND SCRIPT

`login.php` is the login script.
When a user submit a form with the input of username and password, these inputs will be verified against the credentials data stored in the database, if there is a match then the user will be authorized and granted access to site or page.

### HOME PAGE

User is redirected to `home.php` if login is successful.

### PASSWORD RESET

logged in user can reset password for registered account.
script is in `login/password_reset.php`

<hr />
<small>Give this a project ⭐ if you found it useful, and follow me for more interesting future projects</small>

<br>
old images
![SIGN UP](https://user-images.githubusercontent.com/87497268/226151756-a05cb98e-983f-4e14-89f7-be73bce44e49.png)
![LOGIN](https://user-images.githubusercontent.com/87497268/226151758-086f6283-e90a-4da8-820a-1e0c70f71fa3.png)
![WELCOME](https://user-images.githubusercontent.com/87497268/226151762-5e552d91-cfee-4088-9d35-08e03a42b4e8.png)
![RESET PASSWORD](https://user-images.githubusercontent.com/87497268/226151765-d7882815-c780-4966-8ff8-a1b4f6d50f7a.png)
