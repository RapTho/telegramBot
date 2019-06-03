# telegramBot 
This is a code repo that shares my personal telegram bot. The bot is kind of a demo to show IBM's Watson AI services in combination with other third party services. The integration of all services happens on a [Node-RED](https://nodered.org/) server hosted in the [IBM Cloud](https://www.ibm.com/cloud/). All of this is **possible with a free account**

##Requirements
- Free [IBM Cloud](https://www.ibm.com/cloud/) account
- Bot created with Telegram's [Botfather](https://core.telegram.org/bots)
- Free [opencagedata](https://opencagedata.com/) account
- The Telegram messanger installed on your smartphone

##IBM Cloud services
The following IBM Cloud services need to be instinciated. Free/light plan is always sufficient.
- [Watson Assistant](https://www.ibm.com/cloud/watson-assistant/)
- [Watson Visual Recognition](https://www.ibm.com/watson/services/visual-recognition/)
- [Watson Speech-to-Text](https://www.ibm.com/watson/services/speech-to-text/)
- [Watson Language Translator](https://www.ibm.com/watson/services/language-translator/)
- [Weather Company Data](https://cloud.ibm.com/catalog/services/weather-company-data)
- [Node-RED](https://cloud.ibm.com/catalog/starters/node-red-starter)

##Node packages (NPM Modules)
The following modules can be installed directly in Node-RED (npm install)
- node-red-bluemix-nodes
- node-red-contrib-telegrambot
- node-red-node-cf-cloudant
- node-red-node-watson
- node-red-contrib-media-utils
