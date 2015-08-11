#Redis init script to use with Centos 6 /RHEL 6

1. Download and place redis_6379 at /etc/init.d/
2. Adjust the init script with your redis installation config <br>
		redis="/usr/local/bin/redis-server" < change this to where your redis-server installed <br> 
		REDISPORT=6379 < change this with your redis port <br>
		REDIS_CONF_FILE="/etc/redis/${REDISPORT}.conf" < if using port 6379 your config is at /etc/redis/6379 <br>
3. Make it autostart with # chkconfig redis_6379 on
4. Usage : # service redis_6379 start {|stop|status|restart|condrestart|try-restart|reload|force-reload}
