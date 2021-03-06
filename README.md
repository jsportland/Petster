## Petster



## Overview

- The primary function of Petster is to provide a sleek, modern program to facilitate pet adoption matches.
- This will be done by way of a "Tinder"-style interface, allowing prospective adoptors to "swipe" through potential pets.
- The goal is to centralize the process of pet adoption/matching into a single, uniform application.

## Features

- Simple user interface, similar to Tinder/OK Cupid
- Photos/profile for each animal
- Complete available records, including medical, adoption instructions,....

### Tech Stack
|   Back End    |   Front End   |
| ------------- | ------------- |
|    Django     |   Vue.js      |
|    Axios      |   JavaScript  |
|    SQLite     |   Bootstrap 4 |
|               |   HTML        |

**Tasks:**

- Include photos and full-text descriptions of each pet in their 'profile'
- Include all available pet info in 'profile' of pet (background, personality, medical, etc)
- Obtain animal records and store in model/db table
- Allow user to search by details (type,gender,color,etc)
- Include all pertinent contact info, breakdown of costs and procedures for adoption.

> What will the user see on each page?

- A clickable/swipable profile link/picture of the most recently available adoptive pets.
- A search field for specific inquiries
- Selection pulldown box for type of pet to filter

> What can they input and click and see?

- A keyword search for the type/color, etc of pet.
- Each profile can be 'swiped' -either to left or right,

> How will their actions correspond to events on the back-end?

- On left, next animal in list will be displayed,
- On right, animal 'profile' will be loaded

## Data Model

In addition to displaying select information from the api, I will be collecting basic user info for those wishing to maintain a list of favorites to revisit.

### Tables

User Profile:
-name -password -email -location -favorites

Animal Profile:
-animal_id -species_id -breed_id -name -color_id -gender -age -weight -location -photograph -disposition_id -date_entered -date_departed

Species List:
-species_id

Breed List:
-species_id -breed_id

Color List:
-color_id

Disposition List:
-disposition_id -shelter_id
