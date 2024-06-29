EADME
Overview
This repository contains two tasks for web stack debugging and system configuration using Puppet. The tasks aim to improve Nginx server performance under load and fix user login issues due to file descriptor limits.

Task 0: Sky is the Limit, Let's Bring That Limit Higher
Description
This task addresses a high number of failed requests on an Nginx server under load. The goal is to fix the configuration to handle all requests successfully.

Steps
Initial Benchmarking:
Command: ab -c 100 -n 2000 localhost/
Result: 943 failed requests.
Apply Fix:
Command: puppet apply 0-the_sky_is_the_limit_not.pp
Re-Benchmarking:
Command: ab -c 100 -n 2000 localhost/
Result: 0 failed requests.
File
0-the_sky_is_the_limit_not.pp: Puppet manifest to fix Nginx configuration.
Task 1: User Limit
Description
This task resolves the "Too many open files" error for the holberton user, allowing proper login and file access.

Steps
Identify Issue:
Error: /etc/profile: Too many open files.
Apply Fix:
Command: puppet apply 1-user_limit.pp
Verify Fix:
Command: su - holberton
Result: No errors when accessing files.
File
1-user_limit.pp: Puppet manifest to increase file descriptor limits for the holberton user.
Repository Structure
markdown
Copy code
alx-system_engineering-devops/
└── 0x1B-web_stack_debugging_4/
    ├── 0-the_sky_is_the_limit_not.pp
    └── 1-user_limit.pp

