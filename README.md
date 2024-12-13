# Top Board Games, Mechanics and Board Game Designers by Location

# Overview

This project analyzes the top 250 ranked board games on BoardGameGeek.com by pulling each game’s designer(s) and mechanics data from the BGG XML API2. The project will visualize the countries that have designers that have the most highly ranked games, along with the mechanics that appear most often in the top-ranked games.

# Installation
1) Clone Repo to Local Machine
    - Navigate to the folder you would like to clone the repo into.
    - Type: ‘git clone https://github.com/jashel08/board_games_capstone.git’.
2) Create Python Virtual Environment
**IMPORTANT - Make sure that the virtual environment folder is created as '.venv'.**
    - Change directory in Git Bash so the active directory is in the folder created when the repo was cloned.
    - Type ‘python -m venv .venv’.
4) Activate Python Virtual Environment
**IMPORTANT - Make sure you use '.venv' when activating your virtual environment.**
    - On Windows: from the project folder in step 2a, type ‘.venv/scripts/activate’.
    - On Mac: from the project folder in step 2a, type ‘source .venv/bin/activate’.
6) Install Libraries via pip
    - In Git Bash, type: ‘pip install -r requirements.txt’.

# Operation
1) If you have Jupyter Notebook installed, open the ‘Board_Games_Final.ipynb’ file.
2) Run each Python cell from top to bottom, using the run button next to each code block.
3) The end result is the creation of several CSV files, and Pandas Pivot Tables that were used to create Tableau visualizations.

# Tableau Visualizations
Visualizations can be viewed at the following link: [Capstone Tableau Board Game Dashboard](https://public.tableau.com/views/jashel08Capstone-BoardGames/Dashboard1_1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

# Results & Data Interpretation

# Board Game Designers by Country

The United States has produced the most board game designers (100) with board games appearing in the top 250 overall ranked games on BoardGameGeek. While not entirely surprising, I did expect more games with German designers (24) in the top 250, with the birth of modern board gaming having roots there.

# Board Game Mechanics Breakdown

Hand Management is the top mechanic among the top 250 board games, with 88 games containing this mechanic. Given how many games use cards to represent actions, characters, abilities, etc., along with the rise of deck-building games, this isn’t surprising. What was surprising was that 76 games had the Solo/Solitaire game mechanic. I was unaware that solo board gaming had become as popular as this, given the implied social nature of board gaming.

# Top Board Games by Year 

27 board games published in 2019 were in the top 250, followed closely by 2020 with 20. I would have expected to see a drop off in 2020 due to the pandemic, but 2020-2023 all have fairly consistent distributions of top game releases.

# Features

1) Loading Data
    - Read in 2 CSV files
    - Import data to dataframe via API and XML parsing.
2) Clean and Operate on Data
    - Filter out board games with erroneous rank of 0
    - Constrain dataset to top 250 board games.
    - Replace NaN values with ‘0’ or ‘UNKNOWN’ where appropriate.
    - Rounding averages to 2 places.
    - Rename Fields
    - Create pivot tables and csv files based on a cleaned data set.
3) Visualize/Present Data
    - See Tableau Dashboard here: [Capstone Tableau Board Game Dashboard](https://public.tableau.com/views/jashel08Capstone-BoardGames/Dashboard1_1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
    - Pivot tables created in Board_Games_Final.ipynb
4) Best Practices
    - Utilized virtual environment, included instructions for activation.
5) Interpretation of Data
    - Annotated code clearly in markdown cells.
    - Added comments to associate code blocks with steps in markdown cells.

# Sources
1) Boardgame_ranks.csv from BoardGameGeek
2) Board Game Mechanics: BGG XML API 2
3) BGG_Designer_Location.csv - manually created






