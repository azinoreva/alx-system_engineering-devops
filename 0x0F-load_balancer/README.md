ks
0. Double the Number of Webservers
Goal: Configure web-02 identical to web-01
Custom Header: Add X-Served-By with the server hostname in Nginx on both servers
Script: 0-custom_http_response_header
1. Install Your Load Balancer
Goal: Install and configure HAProxy on lb-01
Configuration:
Use round-robin algorithm
Manageable via init script
Proper hostname configuration
Script: 1-install_load_balancer

