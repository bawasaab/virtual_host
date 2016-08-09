# virtual_host

&lt;VirtualHost *:80&gt;
	ServerAdmin test.local
	DocumentRoot "/home/deepak/test/"
	ServerName test.local

	ErrorLog "logs/test.local"
	CustomLog "logs/test.local" common
	
	 &lt;Directory "/home/deepak/test/"&gt;
    		Options Indexes FollowSymLinks
	    	AllowOverride All
    		Order allow,deny
	    	Allow from all
    	&lt;/Directory&gt;
&lt;/VirtualHost&gt;
