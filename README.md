# Video Game Recommendation Dataset

We have prepared dataset for this technical challenge and stored it in Redshift. Refer to messages from recruiting for Redshift connection information and credentials.

This user has an access to:

- database: **`analytics-interview-dataset`**
- schema: **`search-recommendations-system-task`** which contains following tables:
    - **`user_info`**
    - **`video_games`**
    - **`user_games_interaction`**

Description of the tables:

1. **Users (`user_info`)**
    - UserID (unique identifier for each user)
    - Age (age of the user)
    - Gender (gender of the user)
    - Location (location of the user)
2. **Video Games (`video_games` )**
    - GameID (unique identifier for each game)
    - Title (title of the game)
    - Genre (genre of the game, e.g., action, adventure, RPG, strategy, etc.)
    - Publisher (publisher of the game)
    - ReleaseYear (year the game was released)
    - Platform (platform the game is available on, e.g., PC, PlayStation, Xbox, etc.)
3. **User-Game Interactions (`user_games_interaction`)**
    - UserID (references the UserID from the Users table)
    - GameID (references the GameID from the Video Games table)
    - Rating (rating given by the user for the game, on a scale of 1 to 5)
    - PlayTime (total playtime of the game by the user, in hours)
    

### **Connecting to Redshift**

To connect to Redshift, you can use Python with libraries like **`psycopg2`** , **`sqlalchemy`** or **`*redshift_connector`**  by providing connection details in the code. 

Alternatively, tools like SQL Workbench/J, DBeaver or pgAdmin offer graphical interfaces for easier access. Simply input the provided Connection URL, PORT, username, and password into the chosen method's configuration. 

Ensure secure handling of these credentials to protect access to the database. 
Both options facilitate executing queries, managing data, and interacting with Redshift efficiently.
