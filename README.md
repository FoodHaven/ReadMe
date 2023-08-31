<h1>Food Haven</h1>

## Deployed Site: [FoodHaven](https://food-haven.onrender.com/)</h2>

- In a world with food deserts, Food Haven supplies the public with location services for local farmer's markets. The search for markets focuses on farmer's markets that accept Supplemental Nutrition Assistance Program (SNAP) benefits and identifies the type of benefit assistance at the market if the data is available. The user can then select a market they wish to visit and utilizing the maps portion of the application, the user may locate public service transit routes and schedules available to connect them to the market from their current location. 

<b>Developers:</b>

Kailey Kaes: https://github.com/kaileykaes

Jesse Sorman: https://github.com/Jesse193

Kim Bergstrom: https://github.com/kbergstrom78

Andy Stilmock: https://github.com/AStilmock

<h2>FE: https://github.com/FoodHaven/FE_APP</h2>

<h3>For Developers:</h3>

Dependencies: 

Microservice: https://github.com/FoodHaven/microservice-api

Back end: https://github.com/FoodHaven/BE_APP

<h3>Getting started</h3>

Rails Version: 7.0.6

- Run `bundle install` to get all Gems to work properly

- Run `rails db:{drop,create,migrate,seed}`

- Google Oauth 2.0
  - Food Haven features Google Outh as an option to login. When using locally a OAuth client ID and client secret are needed for this to function correctly.
    You can follow the steps to get the required credentials here: https://developers.google.com/identity/protocols/oauth2/web-server
      - Once you have the required credentials make an .env file at the root directory and put the crederntials in that .env file.
        - GOOGLE_CLIENT_ID = YOUR_GOOGLE_CLIENT_ID
        - GOOGLE_CLIENT_SECRET = YOUR_SECRET_KEY
  
<h4>Gems</h4>

- dotenv-rails
  - Documentation for dotenv-rails can be found here: https://www.rubydoc.info/gems/dotenv-rails/2.1.1
     
- omniauth
  - Documentation for omniauth can be found here: https://www.rubydoc.info/gems/omniauth/1.6.1

- omniauth-google-ouath2
  - Documentation for omniauth-google-outh2 can be found here: https://github.com/zquestz/omniauth-google-oauth2
    
- omni-rails_csrf_protection
  - Documentation for omni-rails_csrf_protection can be found here: https://github.com/cookpad/omniauth-rails_csrf_protection

- Faraday
  - Used for HTTP request to APIs 
  - Documentation for Faraday can be found here: https://lostisland.github.io/faraday/#/

- Figaro
  - Used to mask API key(s) from files. 
  - Documentation for Figaro can be found here: https://rubygems.org/gems/figaro/versions/1.1.1
    
- jsbundling-rails
  - Documentation for jsbundling-rails can be found here: https://github.com/rails/jsbundling-rails 



<h2>Microservice: https://github.com/FoodHaven/microservice-api</h2>

- API that consumes USDA snap approved farmer market csv data and exposes that data for backend application consumption.
  - USDA Farmer Markets data table that include farmer markets accepting Supplemental Nutrition Assistance Program (SNAP) Benifits can be found here: (https://www.usdalocalfoodportal.com/fe/datasharing/)

Dependencies: 

Front End: https://github.com/FoodHaven/FE_APP

Back end: https://github.com/FoodHaven/BE_APP

<h3>Getting started</h3>

Rails Version: 7.0.6

- Run `bundle install` to get all Gems to work properly

- Run `rails db:{drop,create,migrate,seed}`

<h4>Gems</h4>

- Geokit
  - Provides geocoding and distance calculation abilities for Ruby on Rails applications.
  - Documentation for Geokit can be found at: https://rubygems.org/gems/geokit
  

<h2>BE: https://github.com/FoodHaven/BE_APP</h2> 
- Consumes the microservice to get SNAP approved farmer markets. <br>


Dependencies: 

Microservice: https://github.com/FoodHaven/microservice-api

Front End: https://github.com/FoodHaven/FE_APP

<h3>Getting started</h3>

Rails Version: 7.0.6

- Run `bundle install` to get all Gems to work properly

- Run `rails db:{drop,create,migrate,seed}`

<h4>APIs</h4>

- Transit
  - Consumes the Transit API to get nearby public transit options and it's details as well as the route(s) available.
  - Transit API requires an API key when used locally. A free API key can be requested at the bottom of the web page here: https://transitapp.com/apis
  - Documentation for Transit API can be found here: http://api-doc.transitapp.com/
    
<h4>Gems</h4>

- Geocoder
  - Used to find geolocation of user in order to find nearby farmer markets that accept SNAP and transit options
  - Documentation for Geocoder can be found here: https://github.com/alexreisner/geocoder
    
- Faraday
  - Used for HTTP request to APIs 
  - Documentation for Faraday can be found here: https://lostisland.github.io/faraday/#/

- Figaro
  - Used to mask API key(s) from files. 
  - Documentation for Figaro can be found here: https://rubygems.org/gems/figaro/versions/1.1.1

- Webmock
  - Used to stub HTTP request
  - Documentation for Webmock can be found here: https://rubygems.org/gems/webmock/versions/3.18.1



