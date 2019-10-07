# Show You Care Park Elsewhere

This application and system allows the reporting of parking incidents, by a member of the public.

They will do this, by scanning a pre-printed sticker with an app on their mobile phone, before placing it on the offending vehicle!

Stickers display a unique QR code, which identifies the incident, and provides a URL.

On discovering the sticker, the perp will find the QR code irresistable! They will scan it with their mobile phone. This will take them to a single page web application, which will inform them of their misdeed, and offer them the opportunity to apologise.

On receipt of an apology, the sevice will send a push notification to the phone which reported he incident.

The phone app source can be found [here](https://github.com/TheAntiParkingCompany/ShowYouCareApp),  with the latest release [here](https://github.com/TheAntiParkingCompany/ShowYouCare/tree/master/releases).  
The API source code, fronting a Postgres database can be found [here](https://github.com/TheAntiParkingCompany/3rd-attempt), with the deployement [here](https://anti-parking-api.herokuapp.com/). You can explore the API, using the Swagger UI, [here](https://anti-parking-api.herokuapp.com/docs).    
The SPWA source code, which provides the sticker generation, and per scanning can be found [here](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers).  

The SPWA deployement for sticker generation can be found [here](https://cerealsuperhero.github.io/SPWA_GenerateStickers/generate/).   
The SPWA deployement which provides the perp scanning, can be found [here](https://cerealsuperhero.github.io/SPWA_GenerateStickers/response/).  


----------

ShowYouCareApp is a web application which we built to show how the JAM Stack works (Javascript, API, Markup). 
It's a pretty simple responsive app which lets anyone logg in an accident through scanning already printed QR code.
You can find the Single Web Page Application for creating Qr code stickers deployed on GitHub [here](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers)

The ShowYouCare App depend on an API, which fronts a database. 

Here is where you can find the code for the [SWPA](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers) and the [App](https://github.com/TheAntiParkingCompany/ShowYouCareApp)

We originally built the project to show the wonder of Platforms-as-a-Service: We used a fantastic service called Restlet, which gave us an online database and UI tools to easily make the RESTFul API to wrap it. Alas Restlet was swallowed by a larger organisation and the service was discontinued. It really helped us though: we could produce a data API in just a few minutes.

**To keep you and your client safe**, here are some ground rules:

* **NO authentication data:** 
  * usernames, passwords
  * shared secrets
  * tokens
* **NO real names** 
  * no personally attributable data of any sort


**Use a gitignore file:** You'll find there is a need only to store a tiny fraction of your source files in a repo. These files depend on the sort of product you are building, and the frameworks you are using. More information (and a selection of gitignore files for common frameworks!) can be found [here](https://github.com/github/gitignore). 

## About this project

Now the project has moved on: we removed the dependency on Restlet, by creating a new API and our own Postgres DB.

Now we'll show you how the RESTful API definition (using the Open API Specification ([which used to be Swagger](https://swagger.io/docs/specification/about/))) we built in Restlet Studio can be used to generate a skeleton server, and a database back-end, without too much more effort.

The result is much more useful, because we can add functionality which transforms the data, rather than just looking it up. Doing more processing on the server means that we reduce the communications traffic, and the processing done on the client.

## How did we do it?

 [Re - implementing the API](https://github.com/aliceliveprojects/WildLoggingDBParent/blob/master/ReImplementing.md) - this shows you how we created a Postgres DB behind the same RESTful API - so we ddn't have to change the client.
 You can see the source codes we used as a guide [here](https://github.com/aliceliveprojects/WildLogging) .
 
