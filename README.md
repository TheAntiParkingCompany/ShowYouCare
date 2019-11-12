# Show You Care Park Elsewhere

This application and system allows the reporting of parking incidents, by a member of the public.

They will do this, by scanning a pre-printed sticker with an app on their mobile phone, before placing it on the offending vehicle!

Stickers display a unique QR code, which identifies the incident, and provides a URL.

On discovering the sticker, the perp will find the QR code irresistable! They will scan it with their mobile phone. This will take them to a single page web application, which will inform them of their misdeed, and offer them the opportunity to apologise.

On receipt of an apology, the sevice will send a push notification to the phone which reported he incident.

The phone app source can be found [here](https://github.com/TheAntiParkingCompany/ShowYouCareApp),  with the latest release [here](https://github.com/TheAntiParkingCompany/ShowYouCare/tree/master/releases).  
The API source code, fronting a Postgres database can be found [here](https://github.com/TheAntiParkingCompany/3rd-attempt), with the deployement [here](https://anti-parking-api.herokuapp.com/). You can explore the API, using the Swagger UI, [here](https://anti-parking-api.herokuapp.com/docs).    
The SPWA source code, which provides the sticker generation, and per scanning can be found [here](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers).

The SPWA deployement for sticker generation can be found [here](https://TheAntiParkingCompany.github.io/SPWA_GenerateStickers/generate/).   
The SPWA deployement which provides the perp scanning, can be found [here](https://TheAntiParkingCompany.github.io/SPWA_GenerateStickers/response/).  


----------

ShowYouCareApp is a web application which we built to show how the JAM Stack works (Javascript, API, Markup). 
It's a pretty simple responsive app which lets anyone logg in an accident through scanning already printed QR code.
You can find the Single Web Page Application for creating Qr code stickers deployed on GitHub [here](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers)

The ShowYouCare App depend on an API, which fronts a database. 

Here is where you can find the code for the [SWPA](https://github.com/TheAntiParkingCompany/SPWA_GenerateStickers) and the [App](https://github.com/TheAntiParkingCompany/ShowYouCareApp)

