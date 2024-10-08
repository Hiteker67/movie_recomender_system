
# Movie Recommender System

## Overview
The **Movie Recommender System** is a content-based recommendation engine that suggests movies to users based on their preferences. It analyzes various aspects of movies, such as genres, cast, crew, and plot descriptions, to determine similarities between different movies. Using this information, the system provides personalized recommendations, offering users a list of the top 5 movies that are most similar to their preferences.

## Features
- **Content-Based Filtering**: Utilizes the content of movies (e.g., genres, plot, actors) to find similar movies, offering recommendations based on what the user has already watched or shown interest in.
- **Top 5 Movie Recommendations**: The system provides the top 5 best recommendations for each movie, helping users find content they'll enjoy quickly and easily.
- **Lightweight and Fast**: Designed for efficiency, the recommender system is lightweight and can easily be integrated into various applications without a significant performance hit.
- **Scalable Design**: Capable of handling a growing movie database, the system is scalable and can be adapted to larger datasets as needed.

## How It Works
1. **Data Collection**:
   - The system uses a dataset that contains detailed information about a large number of movies, including their titles, genres, cast, crew, and plot summaries.
   
2. **Content Processing**:
   - The movie data is processed to extract features such as genres, keywords, and cast. This information is converted into a numerical form that can be used to compare different movies.
   
3. **Similarity Calculation**:
   - A similarity matrix is created by calculating the cosine similarity between the feature vectors of movies. This matrix allows the system to find movies that are most similar to a given movie.
   
4. **Recommendation Generation**:
   - When a user selects a movie, the system uses the similarity matrix to find the top 5 movies that are most similar to the selected movie and presents these as recommendations.
   
5. **Output**:
   - The final output is a list of recommended movies, ranked in order of their similarity to the selected movie.

## Installation
To set up the Movie Recommender System on your local machine, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/movie_recommender_system.git
   ```
   
2. **Navigate to the Project Directory**:
   ```bash
   cd movie_recommender_system
   ```

3. **Install Required Dependencies**:
   - Ensure you have Python installed.
   - Install the dependencies listed in `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application**:
   - Once the environment is set up, you can start the application using:
   ```bash
   python app.py
   ```

## Usage
- **Input**:
  - The user inputs the name of a movie they have watched and enjoyed.
  
- **Output**:
  - The system returns a list of 5 movies that are similar to the input movie based on the content analysis.

Example usage:
```python
 recommend_movies("Inception")
```
Expected Output:
1. Shutter Island
2. The Matrix
3. Interstellar
4. The Prestige
5. Memento

## Project Structure
- **app.py**: The main script that runs the movie recommendation system.
- **movie_dict.pkl**: Contains a dictionary of movies with their corresponding details.
- **movies.pkl**: Stores processed movie data, ready for use in generating recommendations.
- **similarity.pkl**: Contains the similarity matrix used to compare movies.
- **requirements.txt**: Lists the Python libraries required to run the project.
- **setup.sh**: A script to help set up the environment.

## Future Enhancements
- **Collaborative Filtering**: In addition to content-based filtering, implement collaborative filtering to enhance the recommendation accuracy by considering user behavior and ratings.
- **Enhanced Feature Extraction**: Improve the feature extraction process by including more detailed information like directorial style, cinematography, and user-generated tags.
- **Dataset Expansion**: Increase the number of movies in the database, ensuring that the system can offer recommendations across a wider variety of genres and interests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.

## Contributions
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue if you have any suggestions or improvements.

## Contact
If you have any questions or want to reach out, you can contact me at vkc.stw@gmail.com.
