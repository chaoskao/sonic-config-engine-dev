## Introduction
sonic-config-engine-dev is a python project to develop sonic-config-engine, this project also include sonic-py-swsssdk

## setup environment
sudo apt install python-pip  
pip install --upgrade pip  
pip install virtualenv  

## HOWTO
git clone https://github.com/chaoskao/sonic-config-engine-dev.git  
cd sonic-config-engine-dev  
git submodule init  
git submodule update  
cp -r sonic-buildimage/src/sonic-config-engine/ sonic-config-engine

## setup virtual environment
virtualenv --no-site-packages virEnv  
source virEnv/bin/activate

## install dependency
pip install -r requirements.txt

## install sonic dependency
cd sonic-py-swsssdk/  
python setup.py build  
python setup.py install  

## install test dependency
pip install py  
pip install pytest
