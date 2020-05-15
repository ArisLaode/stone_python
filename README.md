# Documentation

General requirements
- ubuntu 18.04.4
- python 3.6.9
- pip 20.1 
- virtualenv 20.0.20
- docker 19.03.6
- npm 3.5.2
- vue 2.6.11

1. Install general requirements

    - $ sudo apt-get install python3-pip
    - $ sudo pip3 install virtualenv
    - $ sudo apt install docker.io
    - $ apt install npm

2. Open teriminal window and run the server-side Flask app with command:

    - $ cd server
    - $ virtualenv -p python3 env
    - $ source env/bin/activate
    - (env)$ pip install -r requirements.txt
    - (env)$ python3 app.py

    Open browser and url http://localhost:5000

4. Open terminal window and run the client-side Vue app with command:

    - $ cd client
    - $ npm install
    - $ npm run serve

    Open browser and url http://localhost:8080

5. Open terminal window to run docker and create a new container
   
    - $ systemctl start docker
    - $ systemctl enable docker

    - pull image nginx & http with command:
    - $ docker pull nginx
    - $ docker pull httpd
    

6. Add container in Vue app:
   - open http://localhost:8080
   - click button -> Add Container
   - input text : nginx , or input text : httpd 
   - click submit
   - note : container have to list from docker pull.

7. check create, running, stop and remove container in options dashboard app.
