 mkdir myapp
 cd myapp/
 python3 -V
 sudo apt-get update
 sudo apt-get install python3-venv python3-pip -y
 python3 -m venv myenv
 source myenv/bin/activate
 nano requirements.txt
 pip install -r requirements.txt
 nano app.py
 gunicorn --bind 0.0.0.0:5000 app:app
 sudo apt-get install nginx -y
 sudo service nginx start
 sudo nano /etc/nginx/sites-enabled/default
 sudo service nginx reload
 gunicorn --bind 0.0.0.0:8000 app:app
