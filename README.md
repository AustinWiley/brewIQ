# BeerKan

A beer tracking app for the professional Brewer and the avid homebrewer that works like a Kanban Board.  BeerKan as a digital Brew log allowing the user to track each batch of beer from raw ingredient to keg. This app is for the Brewer who is always juggling too many batches of beer at a time that he/she cant always remember where in the process every batch is.  Allows the brewer to be more efficient, brew more beer and archive all brewlogs.

## Deployed App

[BeerKan]https://cryptic-fjord-74772.herokuapp.com/)
##

## How it works

### BeerKan has five main streams in its Kan Ban Boord:

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
       * Name of Brewmaster
       * Target Brewing Date
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


 #### NOTE
 * In addition to logging the data to the terminal/bash window, the app will also log the output data to a .txt file called `log.txt`.

### NPM Packages used

   * [Node-Spotify-API](https://www.npmjs.com/package/node-spotify-api)

   * [Axios](https://www.npmjs.com/package/axios)

     * Axios is used to grab data from the [OMDB API](http://www.omdbapi.com) and the [Bands In Town API](http://www.artists.bandsintown.com/bandsintown-api)

   * [Moment](https://www.npmjs.com/package/moment)

   * [DotEnv](https://www.npmjs.com/package/dotenv)

   * [fs](https://www.npmjs.com/package/file-system)
      * Fs is a native node package.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Davey Sjoberg** - *Initial work* - [github](https://github.com/daveysjobey)
* **Daniel Duffy** - *Initial work* - [github](https://github.com/dpd1208)
* **Austin Wiley** - *Initial work* - [github](https://gist.github.com/AustinWiley)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc



### Instructions on how to use Liri-node-app

1. Copy the `liri-node-app` repository to your computer.  Navigate to the root of your project and run `npm install` in a terminal to download the nessesary npm packages.  

2. Next, create a file named `.env`, add the following to it, replacing the values with your API keys for spotify:

```js
# Spotify API keys
SPOTIFY_ID=your-spotify-id
SPOTIFY_SECRET=your-spotify-secret
```
   * This file will be used by the `dotenv` package to set environment variables to the global `process.env` object in node.

   * The Spotify API requires you sign up as a developer to generate the necessary credentials. You can visit                      <https://developer.spotify.com/my-applications/#!/> in order to generate a **client id** and **client secret.**

3. Open a node termial to run the `liri.js` file.

4. liri.js can take in one of the following commands:

   * `concert-this`

   * `spotify-this-song`

   * `movie-this`

   * `do-what-it-says`

### What Each Command Does

1. `node liri.js concert-this <artist/band name here>`

   * This will search the Bands in Town Artist Events API for an artist and render the following information about each event to the terminal:

      ```
       * Name of the venue
       * Venue location
       * Date of the Event
      ```

2. `node liri.js spotify-this-song '<song name here>'`

   * This will show the following information about the song in your terminal/bash window

      ```
       * Artist
       * The song's name
       * A preview link of the song from Spotify
       * The album that the song is from
     ```

    * If no song is provided then the program will default to "The Sign" by Ace of Base.

3. `node liri.js movie-this '<movie name here>'`

   * This will output the following information to your terminal/bash window:

     ```
       * Title of the movie.
       * Year the movie came out.
       * IMDB Rating of the movie.
       * Rotten Tomatoes Rating of the movie.
       * Country where the movie was produced.
       * Language of the movie.
       * Plot of the movie.
       * Actors in the movie.
     ```

   * If the user doesn't type a movie in, the program will output data for the movie 'Mr. Nobody.'

4. `node liri.js do-what-it-says`

  * Using the `fs` Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.

     * It will run `spotify-this-song` for "I Want it That Way," as follows the text in `random.txt`.

     * The text in random.txt can be edited to search movie-this and concert-this as well.

 #### NOTE
 * In addition to logging the data to the terminal/bash window, the app will also log the output data to a .txt file called `log.txt`.

### NPM Packages used

   * [Node-Spotify-API](https://www.npmjs.com/package/node-spotify-api)

   * [Axios](https://www.npmjs.com/package/axios)

     * Axios is used to grab data from the [OMDB API](http://www.omdbapi.com) and the [Bands In Town API](http://www.artists.bandsintown.com/bandsintown-api)

   * [Moment](https://www.npmjs.com/package/moment)

   * [DotEnv](https://www.npmjs.com/package/dotenv)

   * [fs](https://www.npmjs.com/package/file-system)
      * Fs is a native node package.
