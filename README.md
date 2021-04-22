# ChowTime

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Ideas for the Name of App
- ChowTime
- NomNom
- Chewy
- Chefie
- NoMoFrozen

### Description
- Can generate a recipe through calorie count input, bmi input, and ingredient input
- As more users use the app, a feature can be implemented where users can enter in their own recipes
- Filters on what ingredients are necessary, as well as which meal of the day
- Scheduling feature to plan out meals of the week
- Can also list out all possible recipes, and have extra ingredients not entered by a user displayed next to them
- Can also make it so that it generates certain ingredients/recipes based on time of day- for example. if a user uses the app late at night, the app can prioritize quick and easy recipes rather than ones that may require extra ingredients but is more filling

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category: Health and Fitness**
- **Mobile: While the app would start out on and be more user-friendly on mobile devices, the app can later expand to a website in a way similar to apps such as uber eats and grubhub. While these may allow for better availability of our idea, mobile devices may be best suited for making our app as convenient and user friendly as it can be. **
- **Story: Generates recipes through several inputs such as calorie count, health information, and ingredient input. Allows users to input their own recipes as well as schedule their meals throughout the week. Prioritizes time of day and diet to allow for more filtering of recipes that appear on a user's feed to make it more easier for a user to find a recipe that abides to their requirements.**
- **Market: Can be accessed by anyone looking to find a quick meal to create or a place where they can find ingredients others have made. For more advanced features such as calorie count though, it targets those who are looing to abide to specific diets or fitness plans and need a app that can keep track of their calorie count while also providing them with convenient recipes to use.**
- **Habit: This app is meant to adapt to user habit: that is, a user can access it weekly, daily, monthly, or yearly as they can use it whenever deemed necessary or convenient. In the future, we hope to add a calendar feature that would allow users to schedule their meals via the app.**
- **Scope: People would be able to view recipes that abide to their calorie counts, and/or their health information (height, weight, age, etc). In the future, this can be further expanded by showing recipes similar to those favorited by a user on the user's recipe feed. **

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

[x] Login screen w/ Sign Up and Sign In button
[x] Dashboard Screen
    * User can set calorie intake goals for the day
    * User should be able to see saved/recent recipes
    * Retrieve calorie and health information from Apple Watch or fitness tracker?
    * User can see meal suggestions
* Profile page 
    * BMI with Height and Weight
    * Age/Gender
* User must be able to input their available ingredients via manually typing it in or using a camera or photo library
* Saved Recipes
* Recipe Table View which allows users to scroll through recipes
* Recipe Screen for each individual recipe

**Optional Nice-to-have Stories**

* User can be able to favorite their recipes
* Rating System for Recipes
* Calendar View for scheduling meals/recipes

### 2. Screen Archetypes

* Login/Registration Screen
   * User can login and register.
* Dashboard
   * A list of times of when to start making meals
   * Upcoming meals on schedule
   * Calendar for future meals
   * User can customize dashboard screen?
   * Meal suggestions 
* Recipes
    * Users should be able to search for recipes and scroll through an infinite amount of recipes
    * Users should be able to post their own recipes and see them upon pulling down to refresh
* Profile
    * Users can see information such as BMI, calories burnt per day, calorie intake, etc.
* Settings
    * User can switch between light and dark mode
    * User can choose between a selection of various backgrounds
    * Filters to include certain nutrients, ingredients, and calories count.
        * Over time, a BMI filter can be included in as more people post their own recipes 

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Dashboard Screen
* Recipe Screen
* Profile Screen

**Flow Navigation** (Screen to Screen)

* [list first screen here]
   * [list screen navigation here]
   * ...
* [list second screen here]
   * [list screen navigation here]
   * ...

## Wireframes
<img src="https://i.imgur.com/sqOI8ph.png" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 
[This section will be completed in Unit 9]
### Models
#### Users
| Property  | Type | Description
| ------------- | ------------- |--------------
| userID  | String   |Unique ID for the user.
| userImage  | File  | User's profile image.
| userWeight | Number | This integer represents the weight of the user in pounds for use in better filtering out recipes that are fitted for a user's diet or health
| userHeight| Number | This integer represents the height of the user in feet for use in better filtering out recipes that are fitted for a user's diet or health
| userAge | Int | This integer represents the age of the user in years for use in better filtering out recipes that are fitted for a user's diet or health
|favoriteRecipe | Array | Contains the recipes saved/favorited by the user
| healthInfo | Dictionary | Contains daily health-related info for the user (caloriesSpent, caloriesBurnt, calorieGoal)

#### Recipe
| Property  | Type | Description
| ------------- | ------------- |--------------
| recipeID  | String   | Unique ID for the recipe
| timeUsed  | DateTime  | Represents the most recent time the recipe was seen by the user
| ingredients | Array | Contains each of the required ingredients for this recipe in the form of a string
| favorites |Array | Contains a random number of recipes that were favorited by users 
| servingSize | Int | Represents the serving size and adjusts recipe accordingly.### Networking
- Username, recipe, possibly information related to health (weight, height, age) for the recipe screen, the same information but for one user (the one accessing the app) for the profile screen. For the settings screen, information about the type of  backgrounds, calorie/ingredients, etc will need to be pulled 
