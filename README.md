## Introduction
sonic-config-engine-dev is a python project to develop sonic-config-engine, this project also include sonic-py-swsssdk

## download sonic-config-engine
git clone https://github.com/Azure/sonic-buildimage.git  
cp -r sonic-buildimage/src/sonic-config-engine/ sonic-config-engine

## setup environment
sudo apt install python-pip  
pip install --upgrade pip  
pip install virtualenv  

## start virtual environment
virtualenv virEnv  
source virEnv/bin/activate

## install dependency
pip install ipaddr  
pip install netaddr  
pip install PyYAML  
pip install jinja2  
pip install lxml  
pip install natsort

## install sonic dependency
git clone https://github.com/Azure/sonic-py-swsssdk.git  
cd sonic-py-swsssdk/  
python setup.py build  
python setup.py install  

## install test dependency
pip install py  
pip install pytest
