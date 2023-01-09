The Trending page allows the user to discover the Trending movies of the Week and Day. 

The Trending Movies page consists of 3 main features, similar to the home page:
- navbar
- dropdown selection
- card display 

The page uses The Movies Database-TMDB- api

#### i  Navbar:

The navbar is kept the same as the home page, however the Top 10s option contains a dropdown which allows for a quick search of three movie genres that we thought were likely to be the most popular. When clicking on one of these options, the user will be redirected to the top 10 page, and the site will automatically detect if one of the dropdowns are selctected and will render the results on loading the page. Otherwise, if the default dropdown value of Top 10s is selected, the top 10 of all genres will load. 

<p>
    <img src=./assets/img/readme/Navbar-Trending.png>
</p>

#### ii dropdown selection:

-The dropdown provides the user with two search filter options: Day and Week.

-If user click the search button without selecting one of the day/week options, a notification will pop up and disappear after few seconds. 

-once the button is clicked,it will use the TMDB api to fetch for the the top 20 popular movies of the day or week based on user selection.

<p>
    <img src=./assets/img/readme/Navbar-Trending.png>
</p>

#### iii Card Display:

The cards created contain teh following features

- Movie image
- short description of the movie


<p>
    <img src=./assets/img/readme/Navbar-Trending.png>
</p>
