# Last.fm Mixtape Test

A simple test application using Last.fm's free API for building a shareable mixtape app.

## Setup

1. Go to [Last.fm API Account Creation](https://www.last.fm/api/account/create)
2. Create a new app and get your API key
3. Open `lastfm-test.html` in a web browser
4. Enter your API key in the app

## Features

- Search for tracks using Last.fm's free API
- Real-time search without Premium subscriptions
- Add tracks to a personal mixtape
- Export mixtape data (JSON format)
- Display listener counts and popularity

## Current Implementation

This is a prototype using:
- Last.fm Web API (completely free)
- Client-side only implementation
- Local storage for API key
- JSON export for sharing
- Fallback to mock data if API fails

## Advantages of Last.fm

- Completely free API
- No Premium subscription required
- Rich metadata and listener statistics
- Open music database
- Cross-platform music information

## Next Steps

For a production app:
- Backend server for better security
- Database for storing mixtapes
- User authentication
- Social sharing features
- Integration with multiple streaming platforms
- Playlist generation on user's preferred service

## Usage

1. Open `lastfm-test.html` in your browser
2. Enter your Last.fm API key
3. Search for music
4. Add tracks to your mixtape
5. Export/share your mixtape

Note: Uses real Last.fm API with fallback to mock data for demonstration.