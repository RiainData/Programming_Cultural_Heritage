# Programming_Cultural_Heritage
My project for course Programming for Cultural Heritage at the Pratt School of Information.

# Joyce's Works Data Analysis

## Introduction
This Python script is designed to analyze the text files containing James Joyce's works. It performs various tasks such as reading the text files, conducting initial exploration of the data, extracting entities using the NLP library spaCy, and geocoding those entities.

## Part 1: Reading the Text Files
The program reads the following text files:
- Ulysses.txt
- Portrait.txt
- Dubliners.txt

The content of each file is stored in a dictionary for further analysis.

## Part 2: Initial Exploration of Data
1. **Word Counts**: Calculates the total word count for each text file.
2. **Most Common Words**: Identifies the 100 most common words in each text file along with their frequencies.

## Part 3: Using NLP Library spaCy to Extract Entities
The script utilizes the spaCy library to extract entities (locations) from the text files.

## Part 4: Geocoding Entities and Saving to .JSON
1. **Geocoding Process**: Geocodes the extracted locations using the OpenStreetMap API.
2. **Excluded Words**: Specifies a list of words to exclude from the geocoding process to filter out non-location entities.
3. **Output**: Saves the geocoded locations along with their latitude, longitude, and address to a JSON file named 'geocoded_locations.json'.

**Note** GPE refers to Geo-Political Entities, which are typically locations with a defined political or administrative boundary. Examples include countries, cities, states, provinces, and regions. LOC refers to general locations that may not necessarily have a political or administrative boundary associated with them. These can include landmarks, natural features, or generic geographic locations.
In the context of the program, LOC entities represent any other locations mentioned in the text that may not fit the criteria of a GPE but are still relevant for geocoding. 

**Note**: The geocoding process may take significant time to execute, approximately 20 minutes or more due to the nature of the OpenStreetMap geocoding service.

## Usage
1. Ensure Python and the necessary libraries (requests, spaCy) are installed.
2. Run the script.
3. Monitor the progress in the console output.
4. Once complete, the geocoded locations will be saved to 'geocoded_locations.json'.

## Requirements
- Python 
- requests library
- spaCy library

## Author
Riain Fitzsimons
