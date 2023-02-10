---
toc: true
comments: true
title: Project Development
layout: post
categories: [week22]
---

## Overview

What I'm creating for my cpt project will be a tic tac toe game that will be food themed. This will be a place where users can test their tic tac toe skills.

## Purpose and Function

The Purpose is a fun yet competetive way for users to play tic tac toe. Function will be a regular game of tic tac toe that will saves the users score to be able for them to compete against fellow users. The user and user score will be saves in a database that countains the users name and their score that they achieved.

## Data Abstraction

In the Tic Tac Toe game example, data abstraction is achieved by the separation of the backend and the frontend.

In the backend, the game state is stored as a two-dimensional list and the implementation details of how the game state is updated are hidden from the frontend. The frontend only interacts with the backend through a well-defined API endpoint, /game, which allows it to retrieve the current game state and make updates to the game state. The frontend does not have access to the underlying implementation of how the game state is stored or updated in the backend.

## Managing Complexity

The Tic Tac Toe code shows Managing Complexity by separating the backend and frontend and only allowing communication through a well-defined API. This reduces the interdependence of different components and improves maintainability, scalability, and stability by reducing the complexity of the system.

## Procedural Abstraction

The code shows procedural abstraction by encapsulating the implementation details of the game state update logic in the backend, and only exposing the essential information through a well-defined API endpoint. This allows the frontend to interact with the backend in a procedural manner, making updates to the game state without having to be aware of the underlying implementation details.

## Algorithmic Implementation

The code shows algorithmic implementation through the game state update logic in the backend. This logic determines how the game state is updated based on the input received from the frontend and implements the rules of the Tic Tac Toe game. The algorithmic implementation of the game state update is a key part of the overall functioning of the Tic Tac Toe game and allows for a consistent and accurate representation of the game state.

## Testing

I can manualy test using tools like Postman to make API calls to the backend and verify that the correct responses are received.

## Create Performance Task

Each person in our group will be making a food themed game that follows the CPT rubric. These will all be incorparted together into our N@TM project where users can play the different games.

## Code Plan

My tic tac toe game will be coded using HTML/CSS/Python/JavaScript
- The User will be on a Log in screen
- Then they will be on the actual game
- The user can play against a random guest that data wont be saved
- Their score will be saved and be displayed later.

## Video Plan

For the Video I plan to go through the my whole game and show how it will saves the users data. Finally, I would sign and play through a game of tic tac toe and show how the users score will be saved.