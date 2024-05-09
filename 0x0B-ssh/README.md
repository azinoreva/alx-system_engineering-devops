Background Context
This project focuses on enhancing knowledge in server administration, DevOps practices, and security fundamentals. It involves utilizing SSH for remote server access and configuration.

Files Overview
0-use_a_private_key
Bash script to connect to the server using SSH with a private key.
Requirements:
Utilizes ssh with single-character flags.
Connects to the server with the user "ubuntu".
Usage Example:
Copy code
./0-use_a_private_key
1-create_ssh_key_pair
Bash script for generating an RSA key pair.
Requirements:
Creates a private key named "school" with 4096 bits.
Protects the key with the passphrase "betty".
Usage Example:
Copy code
./1-create_ssh_key_pair
2-ssh_config
SSH client configuration file to enable passwordless authentication.
Configuration:
Uses the private key ~/.ssh/school.
Refuses authentication using a password.
Example:
css
Copy code
ssh -v ubuntu@98.98.98.98
3-let_me_in
Instructions for adding a provided SSH public key to the server's authorized keys.
Allows connecting to the server using the provided public key with the user "ubuntu".
100-puppet_ssh_config.pp (Advanced)
Puppet script for configuring the SSH client file.
Requirements:
Configures SSH to use the private key ~/.ssh/school.
Disables password authentication.
Example:
Copy code
sudo puppet apply 100-puppet_ssh_config.pp
