<h1>Food Haven</h1>

<h2>FE</h2>

- Food Haven is an App for people to find nearby USDA Supplemental Nutrition Assistance Program (SNAP) approved farmer markets, and nearby public transportation available.

<h3>For Developers:</h3>

<h4>Gems</h4>

<h2>Microservice</h2>

- API that consumes USDA snap approved farmer market csv data and exposes that data for backend application consumption.
  - The USDA Supplemental Nutrition Assistance Program (SNAP) Benifits list can be found here: https://www.fns.usda.gov/snap/farmers-markets-accepting-snap-benefits

<h2>BE</h2>
- Consumes the microservice to get SNAP approved farmer markets. <br>

<h3>Getting started</h3>

- Run `bundle install` to get all Gems to work properly

- Run `rails db:{drop,create,migrate,seed}`

<h4>APIs</h4>

- Transit
  - Consumes the Transit API to get nearby public transit options and it's details as well as the route(s) available.
  - Transit API requires an API key when used locally. A free API key can be requested at the bottom of the web page here: https://transitapp.com/apis
  - Documentation for Transit API can be found here: http://api-doc.transitapp.com/
    
<h4>Gems</h4>

- Geocoder
  - Used to find geolocation of user in order to find nearby SNAP markets and transit options
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



