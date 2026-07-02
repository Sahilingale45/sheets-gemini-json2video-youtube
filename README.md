# sheets-gemini-json2video-youtube
An advanced programmatic video generation pipeline built on Make.com that takes spreadsheet inputs, drafts data arrays with Gemini AI, renders movies via JSON2Video, and publishes to YouTube.
# Programmatic AI Video Generation & YouTube Publisher Pipeline

This repository contains an advanced Make.com (formerly Integromat) scenario blueprint that automates video asset creation from text-based row inputs to final media delivery on YouTube using AI orchestration and structural video APIs.

## 🚀 How It Works
1. **Trigger (Google Sheets - Watch New Rows):** Pulls structured data, metadata, or topics from a master content sheet on a polling schedule.
2. **Context Design (Google Gemini AI):** Processes the data payload through a generative model to compose detailed scene descriptions, frame properties, or code-friendly JSON arrays.
3. **Data Formatting (Looping Loop):** 
   * **Iterator & Array Aggregator** extract and rebuild elements to format timestamps, assets, text layers, and transition effects.
   * **JSON Modules** handle clean conversions between raw text blocks and JSON schemas.
4. **Rendering (JSON2Video):** Feeds the dynamic configuration file directly into the editing layer endpoint (`Create a Movie from JSON`) and triggers a conditional await loop (`Wait for a Movie to Render`).
5. **Distribution (YouTube - Upload a Video):** Transfers the output binary file asset directly into your channel's uploaded library with predefined titles and descriptions.
6. **Logging (Google Sheets - Update a Row):** Modifies the source sheet line item to flag execution completion and log tracking info.

## 📦 What's Included
* `/blueprints/sheets-gemini-json2video-youtube.json`: The full exported Make.com scenario blueprint configuration file.

## 🔧 Setup Instructions
1. Open your **Make.com** dashboard.
2. Create a new scenario, click the three dots (`...`) located on the bottom navigation control bar, and choose **Import Blueprint**.
3. Upload the `.json` blueprint file from this repository.
4. Establish your account connections:
   * **Google Sheets Modules (1 & 18):** Re-link to your spreadsheet tracking matrix.
   * **Google Gemini AI Module:** Connect using your official Google AI Studio API key.
   * **JSON2Video Modules (21 & 23):** Generate a Project API Key from your JSON2Video dashboard profile and link it.
   * **YouTube Module:** Authorize connection access for your destination Google/YouTube channel handle.
5. Save the configuration and flip the main scheduling toggle switch to **ON**.
