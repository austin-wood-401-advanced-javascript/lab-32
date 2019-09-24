## lab-32 
## Author: Austin Wood

* [Deployed Site](https://nervous-mirzakhani-f8eb89.netlify.com/)

### How this works: 
#### On First Render:
* The app makes a /get call to the Database Server which it takes and populates the list on the screen. 
* The app subscribers to a Q server
#### On form submission: 
* The app makes a /post request to the database server which triggers the server to publish a "create" message
* The Q server hears this publish and publishes another message that the app is listening for. 
* The app takes the payload from the event and appends it to the list it already has on screen, updating the list state.
### Dependencies:
*  @nmq/q
* node-sass
* react
* react-dom
* react-scripts

![UML](https://github.com/austin-wood-401-advanced-javascript/lab-32/blob/master/assets/lab-32UML.jpg)
