# manni

$ git branch
$ git checkout -b manish_beta ………..new beta
$ git clone https://github.com/manav9277/kwapppro.git create clone
$ git checkout -b manish_beta………... for branch




pwd 16011990
esc :wq -----------------quit


sudo mkdir/home/rohit/ecom.imagedb/log

sudo service nginx restart
make supervisor
superviser/conf.d /   sudo vi ecom.conf.d




pull website on git
cd f:
cd git setup
cd/ ecomimagedb
git add
git commit  -m “msg”
git branch
git push origin manish_beta

pull website 


git  clone url of git



make conf.d file

server {
    listen       80;


    */*11111111111111111**********************server_name  kwapp.woo.gy;
    access_log  /home/rohit/kwapppro/log/host.access.log;
    root /home/rohit/kwapppro/;
    location /static {
        alias /home/rohit/kwapppro/static/;
	}
    location /templates {
	alias /home/rohit/kwapppro/templates/;
	}

    location / {
	add_header 'Access-Control-Allow-Origin' *;
	add_header 'Access-Control-Allow-Credentials' 'true';
	add_header 'Access-Control-Allow-Headers' 'Content-Type,Accept';
	add_header 'Access-Control-Allow-Methods' 'GET, POST, OPTIONS, PUT';
        proxy_pass http://127.0.0.1:9004;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
	}

    # Directives turn off 404 error logging.
    location ~* \.(js|css|png|jpg|jpeg|gif|ico)$ {
    	log_not_found off;
	}

   
    error_page   500 502 503 504 404 /50x.html;
    location = /50x.html {
        root   /usr/share/nginx/html;
    }

     
}




make superwisor file
cofn.d file

[program:paymentsimagedb]
command=/usr/local/bin/gunicorn -b "0.0.0.0:9002" --timeout 15 --worker-class gevent -w 2 paymentdb.wsgi 
directory=/home/rohit/paymentsimagedb
redirect_stderr=true
stdout_events_enabled = true
stderr_events_enabled = true


start superwizer
sudo service restart supervisor 



//new diretory pull

cd f:
cd gitstep/
cd kwapp
git pull origin manish_beta
git add.
git commit -m "-"
git push origin manish_beta


// go to putty
go to directory
git pull origin manish_beta
git stash
