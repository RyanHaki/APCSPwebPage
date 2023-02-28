---
toc: true
comments: true
title: Project Development
layout: post
categories: [week22]
---

## Overview

What I'm creating for my cpt project will be a recipe finder where users can type a key word and find a recipe that they desire.

## Purpose and Function

The purpose and the function of this is for users to be able to search any recipe that they like and to be able to find what they want and be givin directions on how to cook the recipe.
## Data Abstraction

The function abstracts these details by simply taking an item name as input, and returning a list of dictionaries that represent the search results for that item. The caller of the function does not need to know the implementation details of how the API is accessed, what query parameters are needed, or how the returned data is formatted, it just needs to know the input and output format of the function.

## Managing Complexity

The code will divided into smaller modules or functions, such as searchItem function, which is responsible for searching an item in the database and returning a list of results.

## Procedural Abstraction

It takes an input item and performs a search on a remote API to retrieve recipe information for that item. The function abstracts away the details of the API request and response handling by encapsulating it in a single function, allowing the user of the function to focus on the task at hand (i.e., searching for recipes) without worrying about the low-level implementation details.

## Algorithmic Implementation

The code will provide a complete implementation of a search API that uses an external API service to retrieve data, parse the data, and return the results in a JSON format.
## Testing

I can manualy test using tools like Postman to make API calls to the backend and verify that the correct responses are received.

## Create Performance Task

Each person in our group will be making a food themed game/feature that follows the CPT rubric. These will all be incorparted together into our N@TM project where users can play the different games and surf through other sites.

## Code Plan

My tic tac toe game will be coded using HTML/CSS/Python/JavaScript
- The User will be on a Log in screen
- Then they will be taken to the rest of the website where they can go to the recipe search
- The recipe finder will only work if users are logged in
- Users will later be able to log out once their done with their searching.
- The account will be saved for later use.

## Video Plan

For the Video I plan to go through the my whole site and show how it will saves the users data. Finally, I would sign and go through my website and be able to search any recipe and then be able to log out.