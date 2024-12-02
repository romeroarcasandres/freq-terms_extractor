# freq-terms_extractor
It processes a text file to extract the most common terms, excluding stopwords, based on the language specified by the user. It outputs a list of the most frequent terms and their counts to a new .txt file.

## Overview
The Frequent Terms Extractor script allows users to select a text file, specify the language of the text, and define how many of the most common words they would like to extract.
The script utilizes natural language processing techniques to tokenize the text, remove stopwords, and calculate the frequency of the remaining words.
The result is a list of the most frequent words and their respective counts, which is written to a new .txt file.

## Requirements:
* Python 3
* tkinter library (for file dialog and user interaction)
* nltk library (for text processing)
  * punkt (for tokenizing the text)
  * stopwords (for filtering out common stopwords)

## Files
freq-terms_extractor.py

## Usage
1. Run the script.
2. A file dialog will prompt you to select a .txt file.
3. After selecting the file, the script will ask:
   * The language of the text (e.g., English, French, Spanish)
   * The number of the most common terms you want to extract.
4. The script processes the text, removing stopwords and non-alphabetic characters, and calculates word frequency.
5. The resulting list of common words and their frequencies will be written to a new .txt file in the same directory as the selected file, and it will have the same name as the original + "_common_terms.txt".
6. The extracted words and their frequencies will also be printed to the console.

## Example Output
intelligence: 10

artificial: 10

Python: 8

## Important Notes
* The text file selected must be a valid .txt file encoded in UTF-8.
* The language provided by the user must correspond to the stopwords available in NLTK. The stopwords specific to the selected language will be removed, ensuring the remaining words are significant for analysis.
* The script is designed to process plain, alphabetic text. Non-alphabetic characters and numbers will be filtered out.

## License
This project is governed by the CC BY-NC 4.0 license. For comprehensive details, kindly refer to the LICENSE file included with this project.

