
# Global Weather Information System

In this application you can deep dive into *Mule 4* using Anypoint Studio to retrieve weather information from SOAP based API running of a separate server .

This application has two main flows, which are further segregated into sub flows. 

The application code follows the best practices some of which are listed below.
   - Modularized RAML file
   - RAML used *triats* and *types*
   - Modularized Mule code
   - Central Configuration file for project
   - Input parameter validation 
   - Flow split into sub for reuse-ability and better code quality
   - Test cases implemented using *Munit*

### Set Up and Run the Application

1. Import the Project global-weather-info-system using Anypoint Studio. 
2. Run the project by right-clicking its main folder and selecting **Run As > Mule Application**.
3. Open any web browser, paste the following URL in the address bar, and press Enter:

        http://localhost:8081/api/globalWeather/getCitiesByCountry?countryName=Australia

      **Result:** Your browser presents a json containing the cities.
   

4. In your browser (or using SOAPUI) address bar, replace the current URL with this one, and then press Enter:

        http://localhost:8081/api/globalWeather/getWeather?countryName=Australia&cityName=Melbourne

      **Result:** Your browser presents a json weather information. 
      


  **Prerequisite:** 
  SOAP web service should be running on the server. 
