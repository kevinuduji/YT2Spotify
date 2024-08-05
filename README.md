# YT2Spotify

### Sample Images 
https://imgur.com/a/ab9u8e5

## Overview

YT2Spotify is a Python tool designed to convert YouTube playlists into Spotify playlists. By leveraging the Spotify API and Google API, this script automates the process of transferring your favorite YouTube music playlists to Spotify, saving you time and effort.

## Features

- **YouTube to Spotify Conversion**: Convert entire YouTube playlists to Spotify playlists effortlessly.
- **Automated Process**: The script handles all the heavy lifting, from extracting video information on YouTube to creating and populating playlists on Spotify.
- **API Integration**: Utilizes the Spotify API and Google API for seamless interaction with both platforms.

## Technologies Used

- **Python**: The primary programming language for the script.
- **Spotify API**: For creating and managing Spotify playlists.
- **Google API**: For accessing YouTube playlist data.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Python (v3.8 or later)
- Spotify Developer Account
- Google Developer Account

### Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/YT2Spotify.git
    cd YT2Spotify
    ```

2. **Create a Virtual Environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

### Setup

1. **Spotify API Setup**:
    - Create a new application on the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
    - Obtain your `Client ID` and `Client Secret`.
    - Add the redirect URI `http://localhost:8888/callback` to your application settings.

2. **Google API Setup**:
    - Go to the [Google Developer Console](https://console.developers.google.com/).
    - Create a new project and enable the YouTube Data API v3.
    - Obtain your API key and OAuth 2.0 credentials.

3. **Environment Variables**:
    Create a `.env` file in the project root directory and add the following:
    ```env
    SPOTIFY_CLIENT_ID=your_spotify_client_id
    SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
    GOOGLE_API_KEY=your_google_api_key
    ```

### Running the Script

1. **Execute the Script**:
    ```bash
    python main.py
    ```

2. **Follow Prompts**:
    - The script will prompt you to authorize the application with Spotify.
    - Provide the YouTube playlist URL you wish to convert.

### Key Components

- **`src/youtube.py`**: Handles interactions with the YouTube API to fetch playlist data.
- **`src/spotify.py`**: Manages interactions with the Spotify API to create and populate playlists.
- **`src/main.py`**: The main script that orchestrates the conversion process.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Kevin Uduji

• [LinkedIn](https://www.linkedin.com/in/kevinuduji/)

• [GitHub](https://github.com/kevinuduji)

---

Thank you for using YT2Spotify! If you have any questions or feedback, feel free to reach out.
