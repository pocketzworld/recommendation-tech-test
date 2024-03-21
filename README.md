## **Objective**

Create a recommendation system that suggests video games to users based on their preferences and behavior.

## **Requirements**

1. **Data Collection and Preprocessing:**
    - Use the dataset provided
    - Preprocess the data to handle missing values, outliers, and ensure consistency.
2. **Model Development:**
    - Design and implement a recommendation algorithm(s) suited for the task (e.g., collaborative filtering, content-based filtering, hybrid methods).
    - Utilize appropriate techniques for feature engineering and representation learning.
    - Implement model evaluation metrics to assess the performance of the recommendation system (e.g., precision, recall, F1-score, mean average precision).
3. **User Interface (Optional but Recommended):**
    - Develop a simple user interface to demonstrate the functionality of the recommendation system.
    - Allow users to input their preferences and view recommended games based on the input.
4. **Documentation:**
    - Provide clear documentation explaining the architecture, design choices, and implementation details of the recommendation system.
    - Include instructions on how to run the system locally or deploy it on a server.
5. **Testing and Deployment:**
    - Conduct thorough testing to ensure the reliability and robustness of the system.
    - If possible, deploy the recommendation system on a cloud platform or local server for demonstration purposes.

## **Deliverables**

1. Python codebase containing the implementation of the recommendation system.
2. Documentation explaining the system's architecture, design choices, and implementation details.
3. Optionally, a simple user interface for interaction with the recommendation system.
4. Test cases and results demonstrating the system's performance.
5. Instructions for running the system locally or deploying it on a server.

## **Evaluation Criteria**

1. **Functionality:** Does the recommendation system effectively suggest relevant video games based on user preferences and behavior?
2. **Scalability:** Is the system scalable to handle a large volume of users and video game data?
3. **Model Performance:** How well does the recommendation model perform in terms of accuracy and relevance of suggestions?
4. **Code Quality:** Is the code well-structured, readable, and maintainable?
5. **Documentation:** Is the documentation clear, comprehensive, and easy to follow?
6. **Bonus:** Any additional features or improvements beyond the basic requirements.

**Note:** Feel free to use any libraries or frameworks you find suitable for the task. Good luck!


----
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

To connect to Redshift, you can use Python with libraries like **`psycopg2`** , **`sqlalchemy`** or **`redshift_connector`**  by providing connection details in the code. 

Alternatively, tools like SQL Workbench/J, DBeaver or pgAdmin offer graphical interfaces for easier access. Simply input the provided Connection URL, PORT, username, and password into the chosen method's configuration. 

Ensure secure handling of these credentials to protect access to the database. 
Both options facilitate executing queries, managing data, and interacting with Redshift efficiently.
