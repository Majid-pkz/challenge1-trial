### **2. Top-10s (Top-10.html)**

The Trending page allows the user to discover the Trending movies of the Week and Day. 

The Trending Movies page consists of 3 main features, similar to the home page:
- navbar
- user 
- card display 

The page uses The Movies Database-TMDB- api

#### i  Navbar:

The navbar is kept the same as the home page, however the Top 10s option contains a dropdown which allows for a quick search of three movie genres that we thought were likely to be the most popular. When clicking on one of these options, the user will be redirected to the top 10 page, and the site will automatically detect if one of the dropdowns are selctected and will render the results on loading the page. Otherwise, if the default dropdown value of Top 10s is selected, the top 10 of all genres will load. 

![2023-01-09 (2)](https://user-images.githubusercontent.com/94885681/211236004-6bedcf1e-7dd6-413a-81ec-68ed35f00e97.png)

#### ii User inputs:

The User inputs provide the user with two simple search filter options. genre and minimum vote count.

- On page load, the script will fetch the list of genres and dynamically create buttons and append the associated value with that button. 

once the user is finished inputting the values they can choose to click the find movies button, which will use the TMDB api to fetch for the the top ten movies that fit into the filtered values and will create card elements of those movies fetched.

![2023-01-09 (5)](https://user-images.githubusercontent.com/94885681/211236367-bb1d0c63-58fd-415d-ae01-b062f7c05204.png)


#### iii Card Display:

The cards created contain teh following features

- Movie title
- Movie rating 
- A short description
- A reviews button 
- A trailer Button 

![2023-01-09 (6)](https://user-images.githubusercontent.com/94885681/211236401-7099df48-fa45-4a25-b558-fd3d1da6abc5.png)

**Reviews button:** 
- use the title appended to the card to redirect to the reviews page, where a review of the chosen movie will appear.

**Trailer button:**
- uses the title appended to the card with a keword 'trailer' added to it to search the youtube database for the most relevant video and executes a function with the video id on a separate API which will generate an iframe and modal for the youtube video to play.  

![2023-01-09 (7)](https://user-images.githubusercontent.com/94885681/211236429-1d716838-5cc9-43db-9c27-1e2dce9bdf31.png)

#### vi Limitations

The TMDB database can occasionally have high rated movies with very low vote counts, meaning that some fetched information will be unreliable, to get around this the minimum vote count is implemented.

The YouTube api can occasionally fetch an irrelevant movie if the TMDB title is different, this only happens in rare cases.
