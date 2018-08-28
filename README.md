# exim-dovecot-auth
Patch for variable server_socket

Variable server_socket can by default accept only UNIX-socket (server_socket = /var/run/dovecot/auth-client).
To use TCP/IP, you need to replace file dovecot.c in the src/auths directory.

Now the variable server_socket can have a value: server_socket = IP:PORT
