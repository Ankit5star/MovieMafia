 # 🎬 MovieMafia — Discover Movies

MovieMafia is a movie discovery website built using **React.js** and the **OMDb API**. It allows users to search for movies and explore their posters, release years, titles, and media types through a clean, responsive interface.

## ✨ Features

- 🔍 **Movie Search:** Search for movies by title.
- 🎞️ **Movie Posters:** Display movie posters with fallback images when unavailable.
- 📅 **Release Year:** View the release year of each movie.
- 🏷️ **Media Type:** Identify whether a result is a movie, series, or another supported type.
- 🎨 **Modern UI:** Dark-themed interface with attractive movie cards and hover effects.
- 📱 **Responsive Design:** CSS styling for desktop and mobile screens.
- ⚡ **Dynamic Data:** Fetch movie information from the OMDb API.
- 🚀 **Default Movies:** Load Batman search results when the application starts.

## 🛠️ Tech Stack

- **Frontend:** React.js, JavaScript (ES6+)
- **Styling:** CSS3
- **API:** OMDb API
- **Development Tools:** Node.js, npm
- **Testing:** Jest and React Testing Library

## 📸 Application Preview

The application features a dark background, a movie search bar, and movie cards containing posters, titles, release years, and media types.

## 📂 Project Structure

```text
MovieMafia/
├── public/
├── src/
│   ├── App.js
│   ├── App.css
│   ├── MovieCard.jsx
│   ├── index.js
│   ├── index.css
│   ├── App.test.js
│   ├── setupTests.js
│   ├── reportWebVitals.js
│   └── search.svg
├── package.json
├── package-lock.json
└── README.md
```

*Note: This structure assumes your uploaded source files are organized inside `src/` in a standard Create React App project.*

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/MovieMafia.git
```

### 2. Navigate to the project directory

```bash
cd MovieMafia
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure the OMDb API

Get an API key from [OMDb API](https://www.omdbapi.com/apikey.aspx).

Create a `.env` file in the project root:

```env
REACT_APP_OMDB_API_KEY=your_api_key_here
```

Update the API URL in `App.js`:

```javascript
const API_URL =
  `https://www.omdbapi.com/?apikey=${process.env.REACT_APP_OMDB_API_KEY}`;
```

Make sure `.env` is included in `.gitignore` and never commit your API key to GitHub.

### 5. Start the development server

```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🔌 API Integration

MovieMafia uses the OMDb API to retrieve movie search results.

Example request:

```text
https://www.omdbapi.com/?apikey=YOUR_API_KEY&s=Batman
```

The application uses the following response fields:

| Field | Description |
|---|---|
| `Title` | Movie or series title |
| `Year` | Release year |
| `Poster` | Poster image URL |
| `Type` | Media type |
| `imdbID` | Unique IMDb identifier |

API documentation: [OMDb API](https://www.omdbapi.com/)

## 🧪 Testing

Run the test suite using:

```bash
npm test
```

Update the default Create React App test in `App.test.js` to match MovieMafia's actual interface before running the tests.

## 🚀 Future Improvements

- Movie details pages with plot, cast, director, and ratings.
- Search by genre, year, and media type.
- Pagination and improved search performance.
- Loading indicators and API error handling.
- Favorites and watchlists.
- Trending and popular movie sections.
- Improved accessibility and mobile navigation.

## 👨‍💻 Author

**Your Ankit5star**

- GitHub: [@Ankit5star](https://github.com/Ankit5star)

## 📄 License

This project is intended for educational and personal portfolio purposes. Add a license file if you wish to specify the terms under which others can use or modify your code.
