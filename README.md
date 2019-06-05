# telegramBot 
This is a code repo that shares my personal telegram bot. The bot is a side project I built combining IBM's Watson AI services and other third party APIs. The integration of all services happens on a [Node-RED](https://nodered.org/) server hosted in the [IBM Cloud](https://www.ibm.com/cloud/).</br>
All of this is **possible with a free account**.

The bot's capabilities shown below can of course be used in many other use cases. So you might wonder what the bot is capable of doing? It can see, hear and understand in a way that resembles us humans. Check out the following demos...

## Recognize objects in images
One of the bot's skills is to see what you see

![Visual Recognition](.ignoreImages/visualRecognition.gif)

## Transcribe user input in different languages
Also, you can dictate your bot something and it will transcribe the spoken words for you. The supported languages are:</br>
English | French | German | Spanish | Japanese | Korean | Mandarin | Arabic

![Speech to Text](.ignoreImages/transcribe.gif)

## Translate between different languages
The bot can also assist you with translations. It will automatically detect which language the input has and translate it to the user desired output language.

![Translate](.ignoreImages/translate.gif)

## Give you a weather forecast at any location
Get the latest weather updates by asking your bot for it. The location is picked from your input and then translated into coordinates by a third party. These coordinates will be used to query the Weather Company's database and return accurate results.

![Weather forecast](.ignoreImages/weather.gif)

# Requirements
- Free [IBM Cloud](https://www.ibm.com/cloud/) account
- Bot created with Telegram's [Botfather](https://core.telegram.org/bots)
- Free [opencagedata](https://opencagedata.com/) account
- The [Telegram messenger](https://telegram.org/) installed on your smartphone

## IBM Cloud services
The following IBM Cloud services need to be instantiated. Free/light plans are always sufficient. No need to add any payment method. Students can get more resources [here](https://ibm.onthehub.com/WebStore/OfferingDetails.aspx?o=142ecca8-0403-e911-810e-000d3af41938).
- [Watson Assistant](https://cloud.ibm.com/catalog/services/watson-assistant)
- [Watson Visual Recognition](https://cloud.ibm.com/catalog/services/visual-recognition)
- [Watson Speech-to-Text](https://cloud.ibm.com/catalog/services/speech-to-text)
- [Watson Language Translator](https://cloud.ibm.com/catalog/services/language-translator)
- [Weather Company Data](https://cloud.ibm.com/catalog/services/weather-company-data)
- [Node-RED](https://cloud.ibm.com/catalog/starters/node-red-starter)

## Node packages (from npm repository)
The following modules are required and can be installed directly in Node-RED (equivalent to "npm install")
- node-red-bluemix-nodes
- node-red-contrib-telegrambot
- node-red-node-cf-cloudant
- node-red-node-watson
- node-red-contrib-media-utils

## Final words
The Node-RED server in this example is hosted on the IBM cloud but it can just as well run on any local device such as a Raspberry Pi or other servers/desktops/laptops as long as they have internet access. Check the [instructions](https://nodered.org/docs/getting-started/installation).

Thanks to Node-RED and the well documented APIs it's really no rocket science. If you want to get started yourself, check out the [build folder](https://github.com/RapTho/telegramBot/tree/master/build) for instructions. Feel free to modify the existing project to your needs. In case you want me to integrate other skills, [send me a message](https://www.linkedin.com/in/raphael-tholl/) and I'll see what I can do.

So far not every possible user exception is caught and dealt with. Since it is just a demo, I left that out for now.
