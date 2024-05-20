
0x0E. Web Stack Debugging #1
Overview
This project focuses on debugging a web stack, specifically dealing with an Nginx installation on Ubuntu 20.04 LTS. Your goal is to ensure Nginx listens on port 80 and is correctly configured to serve web content.

Curriculum
Network Basics
Web Stack DebuggingTask 0: Nginx Likes Port 80
Objective: Fix the issue preventing Nginx from listening on port 80.

Requirements:

Ensure Nginx is running and listening on port 80 of all active IPv4 IPs.
Write a Bash script to automate the configuration.
Script:

bash
Copy code
#!/usr/bin/env bash
# Configure Nginx to listen on port 80
service nginx start
Task 1: Make it Sweet and Short
Objective: Simplify the fix from Task 0.

Requirements:

Bash script must be 5 lines or less.
Maintain usual Bash script requirements.
Avoid using ;, &&, wget, or executing the previous script.
Script:

bash
Copy code
#!/usr/bin/env bash
# Start Nginx service
service nginx restart
Repository
GitHub: alx-system_engineering-devops
Directory: 0x0E-web_stack_debugging_1
Files:
0-nginx_likes_port_80
1-debugging_made_short
