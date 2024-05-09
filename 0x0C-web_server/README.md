Project Overview
Welcome to the ALX System Engineering & DevOps Web Server Curriculum! This repository contains scripts and configuration files for various tasks related to web server setup and management using Nginx on Ubuntu 16.04 LTS.

Project Structure
0-transfer_file
Description: Bash script to transfer a file from a client to a server using scp.
Usage: ./0-transfer_file PATH_TO_FILE IP USERNAME PATH_TO_SSH_KEY
Example:
bash
Copy code
./0-transfer_file some_page.html 8.8.8.8 sylvain /vagrant/private_key
1-install_nginx_web_server
Description: Bash script to install and configure Nginx web server on a Ubuntu machine.
Requirements:
Nginx should listen on port 80.
Querying Nginx at root (/) with a GET request should return a page containing "Hello World!".
Usage: ./1-install_nginx_web_server
2-setup_a_domain_name
Description: Provides a domain name for the server.
Requirements:
Configure DNS records with an A entry to point the root domain to the web server's IP address.
Example:
bash
Copy code
cat 2-setup_a_domain_name
myschool.tech
3-redirection
Description: Bash script to configure Nginx server to redirect requests from /redirect_me to another page.
Requirements:
The redirection must be a "301 Moved Permanently".
Example:
bash
Copy code
curl -sI 34.198.248.145/redirect_me/
4-not_found_page_404
Description: Bash script to configure Nginx server to display a custom 404 page.
Requirements:
The page must return an HTTP 404 error code.
The page content must contain the string "Ceci n'est pas une page".
Example:
bash
Copy code
curl -sI 34.198.248.145/xyz
Usage Instructions
Clone the repository: git clone https://github.com/alx-system_engineering-devops/0x0C-web_server.git
Navigate to the desired task directory.
Run the appropriate script according to the task requirements.
Follow the prompts and instructions provided in the task description for each script.
