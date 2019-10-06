# Show You Care Park Elsewhere

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
 
