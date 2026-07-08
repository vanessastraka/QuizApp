# Mice in Space - QuizApp
Welcome to Mice in Space! 
This is a quiz application built with JavaFX, offering multiple game modes to test your knowledge.
Whether you want to answer random trivia, follow a story, or create your own custom quizzes, this app has something for everyone.

## Features
- **Dynamic Quiz Mode**: Answer trivia questions fetched in real-time from The Trivia API, with adjustable difficulty levels (Easy, Medium, Hard).
- **Engaging Story Mode**: A tutorial that introduces you to the game's theme with a fun narrative about a mouse's journey to space.
- **Customizable Learning Mode**: Create and play your own quizzes by simply uploading a CSV file. A template is provided to get you started.
- **Persistent Highscore Board**: Compete for the top spot! Your scores in Quiz Mode are saved to `data/highscore_data.csv` and can be filtered by difficulty.
- **Secret Mice Mode**: An unlockable, fun easter egg mode for the most dedicated players.
- **Interactive UI**: A clean and user-friendly interface built with JavaFX and styled with custom CSS and a unique font.

## Game Modes Explained
### Quiz Mode
This is the main competitive mode where you test your general knowledge.

- **Questions**: Fetched from [The Trivia API](https://the-trivia-api.com/) for a fresh set of questions every time.
- **Difficulty**: Choose between Easy, Medium, and Hard. This affects the number of lives and the time you have to answer each question.
- **Scoring System**:
    - **Points**: Earn 100 points for each correct answer.
    - **Lives**: Start with 5 lives on Easy, 3 on Medium, or 1 on Hard.
    - **Streak Bonus**: Answering 3 questions correctly in a row grants you an extra life!
- **Highscores**: Your final score is logged on the highscore board.

### Story Mode
This mode serves as a tutorial and introduces the game's theme.

- A guided experience with a fixed set of questions based on a backstory about a brave mouse who dreamed of cheese in space.
- Pop-ups narrate the story as you progress through the questions.

### Learning Mode
Create your own custom quizzes for studying or fun!

1. From the main menu, select **Learning Mode**.
2. **Download the Template** to get a sample CSV file.
3. Open the CSV and add your own questions in the `Question` column and corresponding answers in the `Answer` column.
4. Go back to the app and **Upload** your completed CSV file.
5. The quiz will start automatically. At the end, you can review your performance on the evaluation screen.

### Mice Mode
A hidden game mode where all questions and answers are in "squeak". Unlock it by finding the secret in the main menu!

## Getting Started
### Prerequisites
- Java Development Kit (JDK 17 or higher)

### Running the Application
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/vanessastraka/quizapp.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd quizapp
    ```
3.  **Run the application using the Gradle wrapper:**

    On macOS/Linux:
    ```bash
    ./gradlew run
    ```
    On Windows:
    ```bash
    gradlew.bat run
    ```
The application window will then launch.

## Technologies Used
- **Language**: Java
- **UI Framework**: JavaFX
- **Build Tool**: Gradle
- **UI Definition**: FXML, CSS
- **API**: The Trivia API
- **Data Parsing**: Gson (for JSON)
