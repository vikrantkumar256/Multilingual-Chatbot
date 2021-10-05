# Medchat-voicebot
## _The Multilingual chatbot_

[//]: [![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

Medchat-voicebot is a multilingual chatbot for indian languages built using rasa framework. it provides basic framework/foundation to build multilingual chatbot upon it in any number of languages . 

  Languages supported by medchat and their code is :-
  - English (en-US)
  - Hindi (hi-IN)
  - Marathi (mr-IN)
  - Tamil (ta-IN)
  - Telugu (te-IN)
  - Bengali (bn-IN)
  - Kannad (kn-IN)
 
## Features

- Text chatbot as well as Voicebot
- Applicable for multilanguage
- An easy and convenient framework to build , train and deploy for multilanguage framework .
- Nginx server configured by default for deployment .
- Integrated with Rasa x for local training and sharing chatbot locally .
- Docker used to containerized all the services of Chatbot.
- Simple frontend that takes speech as well as text input.

## Tech

medchat-voicebot uses a number of open source projects to work properly:

- [ReactJS](https://reactjs.org/docs/getting-started.html) - HTML enhanced for web apps! for building frontend.
- [Rasa](https://rasa.com/docs/) - Framework used for building chatbot.
- [Rasa x](https://rasa.com/docs/rasa-x/) - it provides an UI for devlopment , training and sharing locally for intial training of app.
- [Docker](https://www.docker.com/) - used in containerizing application.
- [Nginx](https://www.nginx.com/) - webserver for deployment .
- [jQuery] - duh


## Installation

medchat-voicebot requires python3.6 to run.

Install the dependencies and devDependencies in virtual environment and start the server.

### Development
```sh
cd medchat-voicebot
pip3 install -U pip
pip3 install rasa
pip3 install rasa-x --extra-index-url https://pypi.rasa.com/simple
```
## training
```sh
cd medchatbot-bengali
rasa train nlu
rasa train
```

### using rasa x
```sh
rasa x
```



### Docker

Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 5005, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd medchat-voicebot
sudo docker-compose up
```

it will run expose different port for different services .
as 
- medchatbot-english  http://localhost:5005
- medchatbot-hindi http://localhost:5006
- medchatbot-marathi http://localhost:5007
- medchatbot-tamil http://localhost:5008
- medchatbot-telugu http://localhost:5009
- medchatbot-bengali http://localhost:5010
- medchatbot-kannad http://localhost:5011


