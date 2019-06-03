# telegramBot 
This is a code repo that shares my personal telegram bot. The bot is kind of a demo to show IBM's Watson AI services in combination with other third party services. The integration of all services happens on a [Node-RED](https://nodered.org/) server hosted in the [IBM Cloud](https://www.ibm.com/cloud/). All of this is **possible with a free account**

## Visual Recognition
One skill will be to make your bot see what you see
![Visual Recognition](.ignoreGIFS/visualRecognition.gif)

## Speech to Text
Also you can dictate your bot a text and it will transcribe it for you. Supported languages are:
- English
- French
- German
- Spanish
- Japanese
- Korean
- Chinese (Mandarin)
- Arabic
![Speech to Text](.ignoreGIFS/transcribe.gif)

## Translation
The bot can also assist you with translations. It will automatically detect which language the input text has and translate it to the user desired output language.
![Translate](.ignoreGIFS/translate.gif)

## Weather forecast
Get the latest weather update directly on your smartphone by asking your bot. The location is picked from your input and then translated into coordinates by a third party. These coordinates query the Weather Company database and return accurate results.
![Weather forecast](.ignoreGIFS/weather.gif)

## Requirements
- Free [IBM Cloud](https://www.ibm.com/cloud/) account
- Bot created with Telegram's [Botfather](https://core.telegram.org/bots)
- Free [opencagedata](https://opencagedata.com/) account
- The [Telegram messanger](https://telegram.org/) installed on your smartphone

## IBM Cloud services
The following IBM Cloud services need to be instinciated. Free/light plan is always sufficient.
- [Watson Assistant](https://www.ibm.com/cloud/watson-assistant/)
- [Watson Visual Recognition](https://www.ibm.com/watson/services/visual-recognition/)
- [Watson Speech-to-Text](https://www.ibm.com/watson/services/speech-to-text/)
- [Watson Language Translator](https://www.ibm.com/watson/services/language-translator/)
- [Weather Company Data](https://cloud.ibm.com/catalog/services/weather-company-data)
- [Node-RED](https://cloud.ibm.com/catalog/starters/node-red-starter)

## Node packages (from npm repository)
The following modules are required and can be installed directly in Node-RED (equivalent to "npm install")
- node-red-bluemix-nodes
- node-red-contrib-telegrambot
- node-red-node-cf-cloudant
- node-red-node-watson
- node-red-contrib-media-utils

The subfolders of this repository will explain each skill seperately
