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
    - $ docker create hello-world

6. Add container in Vue app:
   - open http://localhost:8080
   - click button -> Add Container
   - input text -> hello-world
   - click submit

# Note:
  - check docker container in terminal with command:
    - $ docker images 
  - input name container by result docker image. Example, my container: hello-world, so in vue app I have to input my name container "hello-world".
  - you can "start" , "stop" and "romove" in options Vue app.
