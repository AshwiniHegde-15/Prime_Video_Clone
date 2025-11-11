# Prime Video Clone

A web-based streaming platform clone built with Flask and Machine Learning, featuring content recommendations powered by collaborative filtering.

## Features

- **User Authentication**: Secure login and signup system with SQLite database
- **Movie & TV Show Browsing**: Browse movies and TV shows with filtering options
- **Intelligent Recommendations**: ML-based movie recommendation system using cosine similarity
- **Subscription Management**: Multiple subscription tier options
- **Live TV**: Access to live television content
- **Watch History**: Track and manage watched content
- **Responsive UI**: Modern, user-friendly interface with CSS styling

## Project Structure

```
Prime_Video/
├── app.py                      # Main Flask application
├── train.py                    # ML model training script
├── clean_data.py              # Data cleaning and preprocessing
├── netflixdb.py               # Database utilities
│
├── datasets/
│   ├── cleaned_dataset.csv    # Processed movie data
│   ├── movies_dataset.csv     # Raw movies dataset
│   └── movie_links.csv        # Movie links/metadata
│
├── templates/                  # HTML templates
│   ├── home.html              # Home page
│   ├── login.html             # Login page
│   ├── signup.html            # Registration page
│   ├── movies_page.html       # Movies listing
│   ├── tv_shows.html          # TV shows listing
│   ├── live_tv.html           # Live TV page
│   ├── subscriptions.html     # Subscription page
│   ├── watch.html             # Video player page
│   └── payment_success.html   # Payment confirmation
│
└── static/                     # Static assets
    ├── style.css              # Main stylesheet
    ├── subscription.css       # Subscription page styles
    ├── substyle.css           # Additional styles
    ├── watch.css              # Watch page styles
    └── img/                   # Images and assets
```

## Tech Stack

- **Backend**: Flask (Python)
- **Database**: SQLite
- **ML/Data**: Scikit-learn, Pandas
- **Frontend**: HTML, CSS
- **Recommendation Engine**: CountVectorizer, Cosine Similarity

## Installation & Setup

### Prerequisites
- Python 3.7+
- Flask
- Pandas
- Scikit-learn

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/AshwiniHegde-15/Prime_Video_Clone.git
   cd Prime_Video
   ```

2. **Install dependencies**
   ```bash
   pip install flask pandas scikit-learn
   ```

3. **Clean the data**
   ```bash
   python clean_data.py
   ```

4. **Train the ML model**
   ```bash
   python train.py
   ```

5. **Run the Flask application**
   ```bash
   python app.py
   ```

6. **Access the application**
   - Open your browser and navigate to `http://localhost:5000`

## Usage

- **Sign Up**: Create a new account with email and password
- **Login**: Access your account with credentials
- **Browse Content**: Explore movies, TV shows, and live TV
- **Get Recommendations**: View personalized movie recommendations
- **Subscribe**: Choose and manage subscription plans
- **Watch**: Play videos with the built-in player

## Machine Learning Model

The recommendation system uses:
- **CountVectorizer**: Converts text (genre, tags, actor, language) to numerical vectors
- **Cosine Similarity**: Calculates similarity between movies to generate recommendations
- **Features**: Tags, genre, actor, and language information

## Database Schema

The application uses SQLite with the following main table:
- **users**: Stores user credentials and account information
- **recommendations**: Stores movie data and features for ML model

## Future Enhancements

- User ratings and reviews
- Advanced filtering and search
- Payment gateway integration
- Watchlist functionality
- Social sharing features
- Mobile responsive design optimization

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is open source and available under the MIT License.

## Author

**Ashwini Hegde**  
GitHub: [@AshwiniHegde-15](https://github.com/AshwiniHegde-15)

---

*Note: This is a clone/educational project created for learning purposes.*
