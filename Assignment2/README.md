## About this dataset 

![](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.hiclipart.com%2Ffree-transparent-background-png-clipart-pdnhu&psig=AOvVaw0Kfw0BSudyeRlEgSoTX8fY&ust=1763910916658000&source=images&cd=vfe&opi=89978449&ved=0CBUQjRxqFwoTCJCJubCGhpEDFQAAAAAdAAAAABBP<img width="791" height="1011" alt="image" src="https://github.com/user-attachments/assets/6b1f9bc0-9dff-40d0-b599-fe20386e08d0" />
) 


This dataset was collected programmatically from [PokéAPI](https://pokeapi.co), which provides public REST access to Pokémon game data.
It contains the following: 

**ID** – The official Pokédex number.
**Name** – The Pokémon’s English name.
**Types** – All elemental types associated with the Pokémon (e.g., “Fire”, “Water”).
**Document** – An English Pokédex entry retrieved from PokéAPI.
**Filename** – The name of the text file in the data/ folder where the description is stored.
**Doc** - A 'cleaned', preprocessed version of the Document (removing punctuation, normalizing whitespace and lowercasing) 
**Tokens** - The cleaned text seperated per word
**Lemmas** - The tokenized text reduced to their 'roots', their dictionary form  
**POS** - Parts of Speech of all the tokens in this document: the grammatical category the words belong to
**Proper_nouns** - unique persons, places, or things within the descriptions of the Pokémon 

The corpus is part of an exercise carried out in the course Collecting Data in the masters’ program at the University of Groningen. It is intended for use in linguistic analysis and educational purposes.

Each Pokémon description is also saved as a separate .txt file inside the data/ directory for ease of inspection and later processing. The dataset was created automatically by a Python script that queried the PokéAPI for each Pokémon and exported the results into CSV format. The program also handled API response errors (e.g., missing or invalid responses) correctly by skipping over invalid entries. 

Tools used:

* Python
* requests for API access
* pandas for data handling and CSV export
* spaCy for text preprocessing and linguistic annotation

All Pokémon names and descriptions are property of their respective copyright holders. Data was accessed legally via the public PokéAPI under fair use for research and educational purposes.

