0-world_wide_web
This script is designed to configure domain zones and display information about subdomains. It ensures that the subdomains www, lb-01, web-01, and web-02 are correctly configured and points to their respective IP addresses. The script accepts two arguments: domain (mandatory) and subdomain (optional). When only the domain parameter is provided, it displays information for all subdomains. When both domain and subdomain parameters are provided, it displays information for the specified subdomain.

1-haproxy_ssl_termination
This configuration file is for HAproxy, which is set up for SSL termination. It listens on TCP port 443 and accepts SSL traffic. When HTTPS requests are received, it unencrypts the traffic and passes it to the web server. Additionally, it ensures that when querying the root of the domain, the returned page contains "Holberton School".

100-redirect_http_to_https
This configuration file for HAproxy ensures that HTTP traffic is automatically redirected to HTTPS. It returns a 301 status code to transparently redirect users from HTTP to HTTPS, enforcing secure communication. This configuration helps prevent any unencrypted traffic from being served.

These files collectively ensure the proper configuration and secure handling of web traffic through HAproxy for the specified domain. Each file plays a crucial role in achieving the desired functionality and security measures outlined in the tasks.




