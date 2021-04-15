# Microservices Test

## Installation
### Requirements for React
- Node: https://nodejs.org/en/download/
- npm: Installing node automatically installs npm

To check installation, run in terminal,
```
node -v
npm -v
```

### Requirements for Flask
- Python: Will be installed on mac and ubuntu by default

### Requirements for Docker
https://docs.docker.com/engine/install/
---

## Dependencies
### Dependencies for React
Open MicroservicesTest directory in terminal and type the following commands
```
cd test-react-app
npm install axios
```

### Dependencies for Flask
Open MicroservicesTest directory in terminal and type the following commands
```
cd test-flask-app
pip install Flask
pip install flask-cors
```
---

## Running
### Running Flask server
- Running on terminal without docker,
```
cd test-flask-app
python3 -m flask run
```

(Below is the commands if you want to run the flask server using docker)
```
cd test-flask-app
sudo docker build --tag flask-test-docker .
sudo docker run --publish 5000:5000 flask-test-docker
```

### Running React app
```
cd test-react-app
sudo docker build --tag react-test-docker .
sudo docker run --publish 5000:5000 react-test-docker
```
