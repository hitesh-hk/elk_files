# elk_files
Few useful files for ELK 

For "ngnix_logstash.conf" file, do this as well
`nano /var/log/nginx/patterns`
There in the file you need to enter this data

`NGINX_ACCESS %{IPORHOST:remote_addr} - %{USERNAME:remote_user} \[%{HTTPDATE:time_local}\] \"%{DATA:request}\" %{INT:status} %{NUMBER:bytes_sent} \"%{DATA:http_referer}\" \"%{DATA:http_user_agent}\"`
