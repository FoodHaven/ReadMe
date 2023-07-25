<h1>Food Haven</h1>

<h2>FE</h2>

- Food Haven is an App for people to find nearby USDA Supplemental Nutrition Assistance Program (SNAP) approved farmer merkets, and nearby public transportation available.

<h3>For Developers:</h3>

<h4>Gems</h4>


<h2>Microservice</h2>

- API that consumes USDA snap approved farmers markets csv data and exposes that data for backend application consumption.
  - The USDA Supplemental Nutrition Assistance Program (SNAP) Benifits list can be found here: https://www.fns.usda.gov/snap/farmers-markets-accepting-snap-benefits

<h2>BE</h2>

- Consumes the microservice to get SNAP approved farmers markets. <br>
<h4>APIs</h4>

- Consumes the Transit API to get nearby public transit options. As well as the details of the transit option and the route(s) available.
  - Transit API requires an API key when used locally. A free API key can be requested at the bottom of the web page here: https://transitapp.com/apis
  - Documentation for Transit API can be found at: http://api-doc.transitapp.com/
    
<h4>Gems</h4>

- Geocoder
  - Used to find geolocation of user in order to find nearby SNAP markets and transit options
  - Documentation for Geocoder can be found at: https://github.com/alexreisner/geocoder



