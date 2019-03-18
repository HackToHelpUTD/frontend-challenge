## What's the Weather Like? | Frontend Challenge
This fronend challange is for the Hack to Help Frontend Developer Commitee recruitment. Anyone applying to be a frontend developer for Hack to Help must complete this challenge.

### Application Overview
The application that you are required to modify is a weather application that tells the user the current weather based on his/her location. The application gets the geolocation of the user and uses the [OpenWeatherMap](https://openweathermap.org/current) "Current Weather API" to get the current weather by sending over the user's geographical coordinates as parameters to the API call.

The response looks similar to below.

```
{"coord":{"lon":139,"lat":35},
"sys":{"country":"JP","sunrise":1369769524,"sunset":1369821049},
"weather":[{"id":804,"main":"clouds","description":"overcast clouds","icon":"04n"}],
"main":{"temp":289.5,"humidity":89,"pressure":1013,"temp_min":287.04,"temp_max":292.04},
"wind":{"speed":7.31,"deg":187.002},
"rain":{"3h":0},
"clouds":{"all":92},
"dt":1369824698,
"id":1851632,
"name":"Shuzenji",
"cod":200}
```

Parts of this response are parsed and sent over to be displayed to the user. The code responsible for doing this can be found in `src/js/main.js`.

#### Code & Assets
The code and assets follow the following file structure

```
/
---- index.html
---- /src
-------- css/
------------ style.css
-------- imgs/
------------ weather-icons/
---------------- (all weather images in svg)
-------- js/
------------ main.js
```

### Challenge #1
In the API response there is an object called `weather`. It follows the following formatting.

```
"weather":[{"id":804,"main":"clouds","description":"overcast clouds","icon":"04n"}],
```

The key labeled `main` inside the `weather` object is what is being used to determine the icon that will be displayed to the user. Currently the the `main` value is equal to `Clear` the following is displayed.

### Submission
You can either download a zip file and edit that or fork the repo and make your changes there. Whichever way you decide to proceed, make sure to bring in your laptop on the day of your scheduled interview to show us your final result and be prepared to talk through the choices you made. See you soon!

### Questions? Concerns?
Email us at [hacktohelputd@gmail.com](mailto:hacktohelputd@gmail.com).