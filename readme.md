# PAIR: A Pilot Dataset for Duel Perspective-based Video-Grounded Dialogue and Reconciliation

Interactive Knowledge Sharing - Repository

This repository contains a dataset of conversations, structured in both JSON and CSV formats.

## Folder Structure

- `JSON Version/`
  - Contains the dataset in JSON format.
  - File: `pair_dataset.json`
- `CSV Version/`
  - Contains the dataset in CSV format.
  - Subfolders for each video clip ID, each containing three CSV files.

## JSON Version

The JSON file (`pair_dataset.json`) is structured as follows:

### JSON Schema

- **Root Object**: Dictionary containing multiple keys, each representing a unique identifier for a conversation set.
  - Example Keys:
    - `"upenn_0630_Cooking_4_3"`
    - `"indiana_bike_05_5"`
    - `"fair_cooking_08_2"`
    - `"iiith_soccer_001_4"`
    - `"georgiatech_bike_04_10"`
  - **Value**: Array of conversations.

### Each Conversation

- **Array of Message Objects**:
  - **Message Object**:
    - `"Speaker"`: String, indicating the speaker identifier.
    - `"Text"`: String, containing the text of the message.
    - `"Tag"`: String, indicating the tag or dialogue act of the message.

## CSV Version

The CSV version of the dataset is organised into subfolders by video clip ID. Each subfolder contains three CSV files representing three conversations.

### CSV Folder Structure

- **CSV Version/** (Main Folder)
  - **upenn_0630_Cooking_4_3/** (Subfolder for each video clip ID)
    - `Dialogue_01.csv`
    - `Dialogue_02.csv`
    - `Dialogue_03.csv`
  - **indiana_bike_05_5/**
    - `Dialogue_01.csv`
    - `Dialogue_02.csv`
    - `Dialogue_03.csv`
  - **fair_cooking_08_2/**
    - `Dialogue_01.csv`
    - `Dialogue_02.csv`
    - `Dialogue_03.csv`
  - **iiith_soccer_001_4/**
    - `Dialogue_01.csv`
    - `Dialogue_02.csv`
    - `Dialogue_03.csv`
  - **georgiatech_bike_04_10/**
    - `Dialogue_01.csv`
    - `Dialogue_02.csv`
    - `Dialogue_03.csv`

### CSV File Structure

Each CSV file contains the following columns:

- `Speaker`: The speaker identifier.
- `Text`: The text of the message.
- `Tag`: The tag or dialogue act of the message.
