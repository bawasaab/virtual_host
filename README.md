# virtual_host<br>

&lt;VirtualHost *:80&gt;<br>
	ServerAdmin test.local<br>
	DocumentRoot "/home/deepak/test/"<br>
	ServerName test.local<br>
	
	 &lt;Directory "/home/deepak/test/"&gt;<br>
    		Options Indexes FollowSymLinks<br>
	    	AllowOverride All<br>
    		Order allow,deny<br>
	    	Allow from all<br>
    	&lt;/Directory&gt;<br>
&lt;/VirtualHost&gt;<br>
