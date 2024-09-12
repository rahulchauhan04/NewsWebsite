
# News Web App

A responsive and interactive news aggregator web app that fetches the latest news articles from the News API and displays them in a card-based layout. Users can navigate through different news categories or search for specific topics using the search functionality.

## Features

- **News Categories**: Browse news articles related to specific topics like Cricket, India, Technology, and Politics.
- **Search Functionality**: Search for news articles by typing a keyword (e.g., "Science") in the search bar.
- **Dynamic News Display**: News articles are displayed in visually appealing cards that include the article's image, title, source, publication date, and a brief description.
- **Interactive Cards**: Click on a news card to open the full article in a new tab.
- **Responsive Design**: Optimized for various screen sizes, making it accessible on both desktop and mobile devices.

## Technologies Used

- **HTML**: Structure and layout of the web app.
- **CSS**: Styling for the navigation bar, search bar, and news cards.
- **JavaScript**: Fetching data from the News API and dynamically updating the content.
- **News API**: The app uses the [NewsAPI](https://newsapi.org/) to fetch live news articles.

## Setup and Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/news-web-app.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd news-web-app
   ```

3. **Set up the environment**:
   - You need a valid API key from [NewsAPI](https://newsapi.org/). Sign up and get your API key.
   - Replace the `API_Key` in the `script.js` file with your own key.

   ```javascript
   const API_Key = "YOUR_NEWS_API_KEY_HERE";
   ```

4. **Open `index.html`** in your browser to view the app.

## File Structure

```plaintext
├── index.html        # The main HTML file that structures the web app
├── styles.css        # The CSS file that styles the web app
├── script.js         # The JavaScript file that handles API fetching and DOM manipulation
└── logo.png          # The logo used in the navigation bar
```

## Usage

- On page load, the app automatically fetches and displays the latest news articles in the "Technology" category.
- Navigate through the news categories by clicking on any category in the navigation bar.
- Use the search bar to find news related to specific topics by typing keywords and clicking the "Search" button.
- Click on any news card to read the full article in a new tab.

## API

This project uses the [NewsAPI](https://newsapi.org/), which provides access to a wide range of news sources and articles. The app fetches data from the API using this endpoint:

```bash
https://newsapi.org/v2/everything?q={query}&apiKey={API_Key}
```

Where `{query}` is the search keyword (e.g., "Technology", "Cricket", "India", etc.).

## Customization

- You can add more categories or modify the existing ones by editing the `index.html` file in the navigation bar section. Simply update the `<li>` elements with new IDs and modify the `onNavItemClick` function to handle the new categories.
- Adjust the number of articles displayed by modifying the `forEach` loop in the `script.js` file.

## Screenshots

![Screenshot](logo.png)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

