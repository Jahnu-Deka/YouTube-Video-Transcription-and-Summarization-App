# YouTube Video Transcription and Summarization App

Gen AI Project

This project aims to build an end-to-end application that uses Google Gini Pro to transcribe and summarize YouTube videos. The application leverages the YouTube Transcript API to extract the transcript text and Google Gini Pro's generate_content function to summarize the transcript. 

## Table of Contents
- [Project Objective](#project-objective)
- [Key Functionalities](#key-functionalities)
- [Implementation](#implementation)
- [Important Points](#important-points)
- [Installation](#installation)
- [Usage](#usage)
- [Requirements](#requirements)
- [License](#license)

## Project Objective

Build an end-to-end project using Google Gini Pro to transcribe and summarize YouTube videos.

## Key Functionalities
- **Extract Transcript:** Fetch the transcript text from a YouTube video URL using YouTube Transcript API.
- **Generate Summary:** Summarize the transcript using Google Gini Pro's generate_content function.
- **Display Thumbnail:** Show the thumbnail image of the YouTube video.
- **User Interface:** Create a Streamlit app for user input and display results.

## Implementation
1. **Set Up Environment:**
   - Use conda to set up a virtual environment.
2. **Install Libraries:**
   - Install necessary libraries including YouTube Transcript API, Streamlit, and Google Generative AI.
3. **API Key Configuration:**
   - Configure Gini Pro API key.
4. **Streamlit App:**
   - Create a Streamlit app with inputs for the YouTube video URL and a button to trigger summarization.
5. **Define Functions:**
   - Implement functions for extracting the transcript and generating the summary.
6. **Display Results:**
   - Display the video thumbnail and present the summary using markdown.

## Important Points
- Video URLs must be public to extract transcripts.
- The video ID is obtained from the URL by splitting it at the "=" character.
- The transcript is extracted by iterating through the transcript text list and appending it as a paragraph.
- The summary prompt is defined as a variable and appended to the transcript text for summarization.
- Streamlit is used for creating the user interface and displaying the results.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/YouTube_Transcription_Summarization_App.git
    cd YouTube_Transcription_Summarization_App
    ```

2. Create and activate a conda virtual environment:
    ```bash
    conda create -n yt-transcription-summarization python=3.8
    conda activate yt-transcription-summarization
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your Google API key:
    - Create a `.env` file in the project directory.
    - Add your Google API key to the `.env` file:
      ```
      GOOGLE_API_KEY=your_google_api_key
      ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. In the Streamlit interface:
    - Enter the YouTube video URL.
    - Click the "Summarize" button to fetch the transcript and generate the summary.
    - View the video thumbnail and the summarized content.

## Requirements

- Python 3.8
- streamlit
- google-generativeai
- python-dotenv
- youtube-transcript-api

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
