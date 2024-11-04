# This Week in Music 🎶

**This Week in Music**, your go-to app for discovering live music events in your area and listening to curated playlists featuring the artists performing this week!



## Table of Contents

1. [Overview](#Overview)

2. [Key Features](#Key Features)

3. [Installation](#Installation)

4. [Usage](#usage)

5. [Listen to the Playlist](#Listen to the Playlist)

6. [Example](#Example)

   

## 1. Overview

**This Week in Music** helps you stay up-to-date on live concerts and music events happening in your city. It combines event information from the **Ticketmaster** API with **Spotify**'s music library to create personalized playlists based on the week's concerts. Listen to tracks from artists performing near you, discover new music, and get direct access to ticket information.

The purpose of this project is to fetch music events from the Ticketmaster API for a specific date range, location and filter relevant information to classify and analyze event data. The `Spotipy` library enables potential integration with Spotify playlists and artist information.



## 2. Key Features

- **Weekly Event Discovery**: Browse concerts and events happening in your area this week.
- **Custom Playlists**: Enjoy a Spotify playlist generated from the artists performing this week in your city.
- **Event Details**: View event information, including dates and venues.



## 3. Installation

To run this project, ensure you have:

- Python 3.6 or later
- Access to the Ticketmaster API with an API key
- Access to the Spotify API (requires authentication)
- The following Python libraries:
  - `requests` for handling HTTP requests
  - `spotipy` for accessing the Spotify API
  - `nltk` for natural language processing tasks
  - `json` for handling JSON responses
- Creating a virtual environment, `pip install virtualenv`, then activate it.
- After creating a virtual environment, run `pip install -r requirements.txt`



## 4. Usage

To use **This Week in Music**, you'll need API credentials for both Spotify and Ticketmaster. Follow the steps below to set up your environment and start using the app.

#### 1. Get Your API Credentials

##### Spotify API

1. Go to the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).
2. Log in with your Spotify account (or sign up if you don't have one).
3. Click on **Create an App** and provide the required information.
4. Once created, you'll find your **Client ID** and **Client Secret** in the app settings.

##### Ticketmaster API

1. Go to the Ticketmaster Developer Portal.
2. Sign up for an account and create a new app.
3. You'll receive an **API Key** that will allow you to access Ticketmaster's event data.

#### 2. Set Up Environment Variables

To keep your credentials secure, it's best to store them as environment variables. Create a `.env` file in the root directory of the project, and add the following variables:

`SPOTIFY_CLIENT_ID=<Your Spotify Client ID> `

`SPOTIFY_CLIENT_SECRET=<Your Spotify Client Secret> `

`TICKETMASTER_API_KEY=<Your Ticketmaster API Key>`

- **Set up** API keys:

  - Store your Ticketmaster API key in a text file named `ticketmaster_key.txt` in the project directory

  - Set up Spotify credentials in your environment by creating a Spotify developer application [here](https://developer.spotify.com/).

#### 3. Run the Application

After setting up the environment variables, you can run the app to generate playlists based on this week's concerts and events:

1. **Set the Date Range**: Input a `start_datetime` and `end_datetime` for the desired week or timeframe you want to explore.
2. **Fetch Event and Playlist Data**: The app will use the Spotify and Ticketmaster APIs to fetch music data and generate a playlist from artists performing in the specified date range.

The app will then display:

- A list of concerts and events within your selected dates.
- A Spotify playlist featuring songs by artists performing this week, which you can listen to or save directly to your Spotify account.

3. **Browse Events**

After setting the date range, **This Week in Music** will display a list of concerts and music events happening during that period. Each event card includes:

- Event name, time, and venue

  

## 5. Listen to the Playlist

It will generate a Spotify playlist featuring top tracks by artists performing this week.

- **Preview the Playlist**: Click the play button embedded in the app to start listening.
- **Save to Spotify**: If you have a Spotify account, you can save the playlist directly to your Spotify library.



## 6. Example

For example, using **This Week in Music** with a date range of `start_datetime` set to the Monday and `end_datetime` to the following Sunday, the interface connects to both the Spotify and Ticketmaster APIs to identify artists performing in that week. Suppose there are concerts by artists like Glass Animals, ABBA, and some local bands performing at nearby venues. The interface will retrieve music by these artists from Spotify and generate a curated playlist featuring their top tracks. This playlist not only provides users with a tailored listening experience focused on upcoming live music events but also helps them discover and explore artists they can see live in their area that week. Through this example, **This Week in Music** showcases its unique ability to blend event discovery with personalized music streaming into a seamless, real-time experience.



<iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/09NlA0BVdE7Y0vfa4jpw1l?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

Enjoy exploring the music scene around you with **This Week in Music**! 🎸🎤🎻

