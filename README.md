# This or That Game: Dog Image Voting System

## Project Overview

Our project is a web-based **"This or That"** game where users are presented with two dog images and select their favorite. Once a selection is made, the system fetches two new random images, ensuring a continuous and engaging experience. The votes are recorded in a database, allowing us to track the most popular dog images. Additionally, a leaderboard displays the top 10 highest-voted images.

## Tech Stack

- **Frontend:** A simple, clean, and visually appealing interface built with **Vue.js** for fast development and smooth user interactions.
- **Backend:** **Node.js** with **Express.js** for handling API requests and managing data flow.
- **Database:** **MongoDB** for storing votes and tracking the most popular dog images.
- **Image Source:** [Dog CEO API](https://dog.ceo/api/breeds/image/random) for fetching random dog images.

## Features & Implementation

### Core Features:

#### Image Selection:

- Users see two randomly fetched dog images.
- They select their favorite with a click.
- The system immediately replaces them with two new random images.

#### Vote Tracking:

- Each image's selection count is stored in MongoDB.
- The backend assigns a unique identifier to each image for accurate vote tallying.

#### Leaderboard:

- Displays the top 10 most-voted dog images.
- Dynamically fetches data from the database.

#### Smooth Animations:

- Transitions between images include smooth fade-in and fade-out effects.

### Backend Implementation:

- A Node.js server with Express.js handles API requests.
- **Routes include:**
  - `GET /images`: Fetches two random images from the Dog CEO API.
  - `POST /vote`: Records a vote for a selected image.
  - `GET /leaderboard`: Retrieves the top 10 most-voted images from MongoDB.
- **MongoDB storage:**
  - Image URLs with unique IDs.
  - Vote counts for each image.

### Frontend Implementation:

- Built with Vue.js for fast and efficient development.
- Calls backend APIs to fetch images and leaderboard data.
- Displays images in a visually appealing layout.
- Incorporates animations for smooth transitions between images.
- Provides an interactive and responsive user experience.

## Conclusion

This project demonstrates a simple yet engaging application that incorporates external APIs, database interactions, and real-time user choices. It not only allows users to engage with adorable dog images but also tracks and showcases the most popular ones, creating a fun and interactive experience. The implementation ensures a smooth and efficient workflow, leveraging modern web technologies for an enjoyable user experience.
