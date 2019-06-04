# Complete flow
![Node-RED flow](../.ignoreImages/node-red_complete_flow.png)

This is the complete flow as I use it. Credentials of the Watson AI nodes have been removed. Also the API key of the http call to opengatedata, which translates the location from word to coordinates, has to be modified the following way:

```
msg.url = "https://api.opencagedata.com/geocode/v1/json?q=" + msg.loc + "&key=REPLACE_WITH_YOUR_APIKEY&language=en&pretty=1"
return msg;
```
The variable in REPLACE_WITH_YOUR_APIKEY in the URL has to be replaced with your individual API key that you receive after registering at [opencagedata.com](https://opencagedata.com/)

The function node right before the "http get request node" carries the code shown above.
