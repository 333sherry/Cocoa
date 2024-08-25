# Cocoa (Our Team Name)
This NYC food and in-theater movie guide was made in NYU's Project for Programming 2024 Spring class. Sample video link: https://drive.google.com/file/d/1pSCpyxaVH3Y7GPd2ZcPiXfe_rClH1o97/view?usp=sharing

## Project Description
### Our Goal
Our project aims to create a personalized recommendation system for individuals or groups of users to find new and exciting restaurants to explore and in-theater movies to watch in New York City. 

This project has a platform for restaurant recommendations where users can build food preference profiles that record their preferences for different cuisines. Based on their individual preferences, our project will provide weekly recommendations across several food establishment categories. We also created a system that can input multiple user preference profiles to generate recommendations suitable for everyone in groups of two or more individuals. This feature will help plan dates or friend group hangouts where everyone has different tastes but wants to get food together. 

For the in-theater movie recommendation, we have a movie recommender system designed for movie enthusiasts who want to find movies that match their preferences. To offer personalized recommendations, the system uses natural language processing to analyze users' preferred genres and past movie experiences. It uses the Gemini AI model and our movie database to identify relevant current in-theater movies matching user preferences. Users can input their favorite genres or movies using the simple web interface, and the system will generate a comprehensive list of current movies in New York City theaters. The list includes summaries and links to make it easier for users to choose, aiming to help users find movies they like and enhance their movie-watching experience.

### Data Collection
We have collected data primarily from Yelp, NYC Open Data, and Rotten Tomatoes. Our project’s process of fetching activity data entails scraping the listed websites below (with suitable functions for each domain) into a Pandas data frame, cleaning it up by removing duplicates and columns we do not need from data sets, and storing it in the corresponding category’s SQL table within our database. We scraped Yelp for information on establishments like restaurant categories (what we refer to as “tags” throughout the code), phone numbers, images, website links, etc. We scraped Rotten Tomatoes for information on movie titles, poster images, audience ratings, etc.

#### Data Sources
+ Time Out 
+ NYC Restaurant Inspections 
+ City Guide NY Restaurants    
+ Eater NY
+ Resy 
+ Yelp API 
+ OpenWeatherMap
+ Rotten Tomatoes
+ Fandango
+ Kaggle

### Approach
We approached the recommendation system by breaking the process down into several steps:
1. Gathering activity data into a SQL database (food + movie) through web scraping 
2. Filling in missing activity information, such as addresses, price range, etc., through APIs
3. Collecting user input (explicit preferences stated by the user and provided reviews of recommended places to eat)
4. In our milestone, we used profiles created by ChatGPT as we do not have any users yet to develop recommendations for
5. Building user profile preferences based on inputs
6. Leveraging the extensive and up-to-date database and user preference data to suggest personalized recommendations
7. Analyzing preferences of multiple user profiles (various sets of input data) to offer ideas for groups looking for places to eat together through clustering and dendrograms
8. Run the Machine Learning Model
9. Recommend in-theater movies using Gemini AI with the resulting markdown table and user inputs
10. As a user interacts with the system and provides feedback on the system’s recommendations, it will learn and tailor results to align more with the user’s preferences
11. As time passes, the activity database will continue growing and updating with time-limited or currently trendy restaurants to recommend to users

## Group Member Contacts
Since not all members have a GitHub account, our group members' first names and contacts are here.
+ Sherry: mx2046@stern.nyu.edu
+ Alice: jac10027@stern.nyu.edu
+ Casey: cgr9215@stern.nyu.edu
+ Jessica: jro323@stern.nyu.edu
+ Tanisha: tr2095@stern.nyu.edu
