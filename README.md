# virtual_host

<VirtualHost *:80>
	ServerAdmin test.local
	DocumentRoot "/home/deepak/test/"
	ServerName test.local

	ErrorLog "logs/test.local"
	CustomLog "logs/test.local" common
	
	 <Directory "/home/deepak/test/">
    		Options Indexes FollowSymLinks
	    	AllowOverride All
    		Order allow,deny
	    	Allow from all
    	</Directory>
</VirtualHost>
