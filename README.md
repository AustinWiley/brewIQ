# BeerKan

Beer tracking app for the professional brewer and the avid homebrewer that works like a Kanban Board.  BeerKan as a digital Brew log allowing the user to track each batch of beer from raw ingredient to keg. This app is for the Brewer who is brewing multiple batches at a time with batches at different stages of the process.  Allows the brewer to be more efficient, brew more beer and archive all brewlogs.

## Deployed App

Deployed on Heroku using the JAWS_DB add-on for the MYSQL databes.  

#### Click Here: [BeerKan](https://cryptic-fjord-74772.herokuapp.com/)
##

## How it works

### BeerKan has five streams in its Kan Ban Boord:

   * `Create A new Beer`

   * `Inventory`

   * `Brew In-process`

   * `Distribution`
   
   * `Archive`

### What Each Stream Does

1. `Start a new Beer`

   * This will allow you create a new card with the following information:

      ```
       * Name of the beer
       * Style
       * Name of Brew Master
       * Target Brew Date
      ```
  `add gif here!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`
  
2. `Inventory`

   * This will is where you can plan out your beer before brew day with all the info necessary for prep:

      ```
       * Ingredients
       * Fermantaion Tank 
       * units of mesurement
       * notes
     ```
  `add gif here!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`
  
3. `Brew In-process`

   * This is where you will track the beer from Wort production to fermented beer including:

     ```
       * Brew House Targets and efficiencies.
       * Yeast Management.
       * Fermentation.
       * Dry Hopping.
       * Cellaring.
     ```
  `add gif here!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`
  
4. `Distribution`

   * This is where you will track:

     ```
       * Transfer Dates.
       * Bright tank location.
       * Racking(kegging) information.
       * Volumes.
     ```
  `add gif here!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`

4. `Archives`

   * This is where you can view all of the previously entered information on past batches of beer:

     ```
      * This part of the project is still under construction.
     ```
      

  `add gif here!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`

 ## Future Development
  Future build out of the app could include: 
 * Compleation of Archives Section
 * Track Daily specific Gravity and display fermentaion progress on a graph
 * Creat timed alerts to keep you on schedule
 * Ability to print a pdf of the Brew log
 * Ability to pull reports in a printable pdf format that will assist in calculating federal and local excise taxes
 * Creat and add a tool that performs common brewing calultions that include:
    * Alpha Acid Hop Adjustments
    ** O.G. Gravity adjustments
    ** ABV Calculator
    ** IBU Calculator
    ** Yeast Pitch rate Calculator
    ** And more

## NPM Packages used

   * [Node-Spotify-API](https://www.npmjs.com/package/node-spotify-api)

   * [Axios](https://www.npmjs.com/package/axios)

     * Axios is used to grab data from the [OMDB API](http://www.omdbapi.com) and the [Bands In Town API](http://www.artists.bandsintown.com/bandsintown-api)

   * [Moment](https://www.npmjs.com/package/moment)

   * [DotEnv](https://www.npmjs.com/package/dotenv)

   * [fs](https://www.npmjs.com/package/file-system)
      * Fs is a native node package.

## Built With
The App was build by team collaboration using a Scrum board to track our progress with the goal of a MVP within a two week sprint. 
* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Authors

* **Davey Sjoberg** - [github](https://github.com/daveysjobey)
* **Daniel Duffy** - [github](https://github.com/dpd1208)
* **Austin Wiley** - [github](https://gist.github.com/AustinWiley)

See also the list of [contributors](https://github.com/daveysjobey/brewIQ/graphs/contributors) who participated in this project.

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
