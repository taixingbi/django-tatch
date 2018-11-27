## start from aws

1. access aws      
chmod 400 keypair-django.pem       
sudo ssh -i "keypair-django.pem" ec2-user@ec2-18-218-141-159.us-east-2.compute.amazonaws.com    

2. set up django   
virtualenv venv     
source venv/bin/activate    
pip install Django==1.8.1    
pip freeze > requirements.txt    
pip install -r requirements.txt   

3. start  
python manage.py runserver 0.0.0.0:8000    
18.218.141.159:8000

## start django
virtualenv venv     
source venv/bin/activate        
cd mysite        
python manage.py runserver      

## refresh static files
python manage.py collectstatic --noinput --clear    
clear browse cookies   

## setup env

pip install virtualenv

virtualenv venv

source venv/bin/activate

pip install Django==1.8.1

pip freeze > requirements.txt

pip install -r requirements.txt


## setup django app

django-admin startproject mysite

cd mysite    
//setup myapp         
python manage.py startapp myapp       
  
//setup database       
python manage.py migrate         

python manage.py runserver




## reference
[1] [Django Intro Tutorial! Build a website in 11 mins](https://www.youtube.com/watch?v=PqeAvFf_HDI)      
[2] [startbootstrap](https://startbootstrap.com/)
