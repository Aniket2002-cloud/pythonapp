*Following Steps off python app hosting*

1)  mkdir myapp

2)  cd myapp/

3) python3 -V

4) sudo apt-get update

5) sudo apt-get install python3-venv python3-pip -y

6) python3 -m venv myenv

7) source myenv/bin/activate

8) nano requirements.txt

9) pip install -r requirements.txt

10) nano app.py

11) gunicorn --bind 0.0.0.0:5000 app:app

12) sudo apt-get install nginx -y

13) sudo service nginx start

14) sudo nano /etc/nginx/sites-enabled/default

15) sudo service nginx reload

16) gunicorn --bind 0.0.0.0:8000 app:app
