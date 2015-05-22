WNPM2.0配置：

server {

> listen       80;

> server\_name  thinkphp.items.10.con;

> root         /svnroot/items/thinkphp/;

> index        index.html index.htm index.php;

> charset      utf-8;

> access\_log  off;


> location ~ \.php {

> fastcgi\_pass   127.0.0.1:9000;

> set $path\_info "";

> set $real\_script\_name $fastcgi\_script\_name;

> if ($fastcgi\_script\_name ~ "^(.+?\.php)(/.+)$") {

> set $real\_script\_name $1;

> set $path\_info $2;

> }

> fastcgi\_param SCRIPT\_FILENAME /svnroot/items/thinkphp/$real\_script\_name;

> fastcgi\_param SCRIPT\_NAME $real\_script\_name;

> fastcgi\_param PATH\_INFO $path\_info;

> include        /wnpm/webserver/nginx/conf/fastcgi\_params;

> index        index.php;

> }

}



WNPM1.0配置：

server {

> listen       80;

> server\_name  thinkphp.items.10.con;

> root         /svnroot/items/thinkphp/;

> index        index.html index.htm index.php;

> charset      utf-8;

> access\_log  off;


> location ~ \.php {

> fastcgi\_pass   127.0.0.1:9000;

> set $path\_info "";

> set $real\_script\_name $fastcgi\_script\_name;

> if ($fastcgi\_script\_name ~ "^(.+?\.php)(/.+)$") {

> set $real\_script\_name $1;

> set $path\_info $2;

> }

> fastcgi\_param SCRIPT\_FILENAME /svnroot/items/thinkphp/$real\_script\_name;

> fastcgi\_param SCRIPT\_NAME $real\_script\_name;

> fastcgi\_param PATH\_INFO $path\_info;

> include        /usr/local/webserver/nginx/conf/fastcgi\_params;

> index        index.php;

> }

}