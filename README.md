<h1>Food Haven</h1>

- Food Haven is an App for people to find nearby farmer markets that accept Supplemental Nutrition Assistance Program (SNAP), and nearby public transportation available.

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

<h4>Gems</h4>

- Faraday
  - Used for HTTP request to APIs 
  - Documentation for Faraday can be found here: https://lostisland.github.io/faraday/#/

- Figaro
  - Used to mask API key(s) from files. 
  - Documentation for Figaro can be found here: https://rubygems.org/gems/figaro/versions/1.1.1


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



