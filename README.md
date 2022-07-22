### Template for starting wordpress with compose and nginx php fpm without any wordpress images. 

This repo is cloned by a bash script to automatically sccafold folder structure required, files will be copied,
wordpress code will be cloned by the bash script and domain name is replaced with the user input[domain name]
to generate ssl certificates using certbot.

It should be kept in mind that when you start the compose first time you should comment out 443
block in default.conf and 301/302 block also so that the certificates can be generated for the first time,

and then you can uncomment those 443 server blocks once the certificates are generated at required volume.

bash script can be found at ->>> https://github.com/gouravthakur39/generate-wp-bash-script
