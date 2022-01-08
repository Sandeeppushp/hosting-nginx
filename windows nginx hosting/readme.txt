Download the nginx for windows(stable) from here: http://nginx.org/en/download.html
got to conf folder and edit nginx.conf file
make ssl folder and put key and crt file
open cmd and run nginx.exe


Check and make sure 443 and 80 ports are open


in Case of PFX file, use below commands:
openssl pkcs12 -in ncom.pfx -nocerts -out keyfile-encrypted.key
openssl pkcs12 -in ncom.pfx -clcerts -nokeys -out certificate.crt
openssl rsa -in keyfile-encrypted.key -out keyfile-decrypted.key


