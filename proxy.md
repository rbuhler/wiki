listar proxys:

git config --global -l 

=======SETUP PROXY===================

git config --global http.proxy http://proxy.wdf.sap.corp:8080

git config --global https.proxy http://proxy.wdf.sap.corp:8080


npm config set proxy http://proxy.wdf.sap.corp:8080

npm config set https-proxy http://proxy.wdf.sap.corp:8080


set HTTPS_PROXY=http://proxy.wdf.sap.corp:8080

set HTTP_PROXY=http://proxy.wdf.sap.corp:8080

set ALL_PROXY=http://proxy.wdf.sap.corp:8080

===============REMOVE PROXY=================

git config --global --unset http.proxy

git config --global --unset https.proxy

npm config rm proxy

npm config rm https-proxy

set HTTPS_PROXY=

set HTTP_PROXY=

set ALL_PROXY=
