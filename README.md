# (re)Install WordPress
A simple playbook that will:
- Install from scratch the latest WordPress
- Drop all tables from the current MySQL/MariaDB database
- Generate and use a new table_prefix, unique keys, and salts
We assume that MySQL/MariaDB and web server software are already installed and in use.

## Requirements
- Web server is installed
- MySQL or MariaDB is already installed
- WordPress installation path is already used or defined in web server configs

## Playbook Variables

    install_path: "/set/path/to/the/public_html"
    db_name: "database_name_here"
    db_user: "database_dbuser_name"
    db_pass: "database_dbuser_password"
    db_host: "localhost"

## How to run a playbook

    ansible-playbook -i hosts.ini install-wordpress.yml

## Author Information
Darko Drazovic \
LinkedIn: https://www.linkedin.com/in/darkodrazovic \
Personal: https://darkodrazovic.in.rs \
Blog: https://kompjuteras.com \
GitHub: https://github.com/darkodrazovic
