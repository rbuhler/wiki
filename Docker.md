# DOCKER

## VAGRANT
[Download](https://www.vagrantup.com/)

## IMPLEMENTATION STEPS
-----------------------
`sudo nano /etc/environment`

```
ALL_PROXY  = http://proxy.wdf.sap.corp:8080
HTTP_PROXY = http://proxy.wdf.sap.corp:8080
HTTPS_PROXY = http://proxy.wdf.sap.corp:8080
NO_PROXY = *.local,169.254/16,*.sap.corp,*.corp.sap,.local,.sap.corp,.corp.sap,*.cloud.sap,.cloud.sap
```

`sudo nano /etc/apt/apt.conf`
```
Acquire::http::proxy "http://proxy.wdf.sap.corp:8080";
Acquire::https::proxy "https://proxy.wdf.sap.corp:8080";
Acquire::ftp::proxy "ftp://proxy.wdf.sap.corp:8080";
```

`sudo apt-get install docker.io`

docker --version

* https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html
  `docker pull docker.elastic.co/elasticsearch/elasticsearch:5.4.1`

* Issue with proxy:
  `https://stackoverflow.com/questions/23111631/cannot-download-docker-images-behind-a-proxy`
  
  ### Done till here!

