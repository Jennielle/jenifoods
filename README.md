# Recipe Finder

Recipe Finder is a React-based application that allows users to search for recipes and view detailed information about their favorite dishes. It utilizes the Edamam Recipe Search API to fetch recipes based on user input, and it displays them in a modern, user-friendly interface.

## Features

- **Search Recipes:** Find recipes by entering a search term.
- **Detailed Ingredients:** View a list of ingredients for each recipe in a modal.
- **Styled Interface:** Built with styled-components for custom styles and Material-UI for modals.
- **Real-Time Search:** Implements debouncing to fetch data efficiently as users type.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Technologies Used

- React
- Axios
- Styled-Components
- Material-UI
- Edamam Recipe Search API

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/jennielle/Recipe Finder.git
   cd Recipe Finder
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Add your Edamam API credentials:
   - Obtain your API ID and API Key from [Edamam](https://developer.edamam.com/).
   - Replace the placeholders in `App.js` with your credentials:
     ```javascript
     const APP_ID = "your-app-id";
     const APP_KEY = "your-app-key";
     ```

4. Start the development server:
   ```bash
   npm start
   ```

5. Open [http://localhost:3000](http://localhost:3000) to view the app in the browser.

## Folder Structure

```
Recipe Finder/
├── public/
│   └── ... (static assets like index.html, icons)
├── src/
│   ├── App.js          # Main application logic
│   ├── index.js        # Entry point for React
│   ├── index.css       # Global styles
│   ├── package.json    # Project metadata and dependencies
├── README.md      # Project documentation
└── yarn.lock      # Dependency lockfile
```

## How to Use

1. Type a recipe or ingredient name in the search bar.
2. Click on a recipe to view its ingredients.
3. Open the full recipe in a new tab by clicking "See Complete Recipe."

## API Reference

The app uses the Edamam Recipe Search API:
- **Endpoint:** `https://api.edamam.com/search`
- **Parameters:**
  - `q` (string): Search query.
  - `app_id` (string): Your API ID.
  - `app_key` (string): Your API Key.

Example:
```bash
https://api.edamam.com/search?q=pasta&app_id=your-app-id&app_key=your-app-key
```

## Contribution Guidelines

1. Fork the repository.
2. Create a new branch for your feature or bugfix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes with descriptive messages:
   ```bash
   git commit -m "feat: add feature description"
   ```
4. Push to your forked repository and create a pull request.

## Git Commit Conventions

Use the following format for commit messages:

- `feat:` For new features (e.g., `feat: add search functionality`).
- `fix:` For bug fixes (e.g., `fix: resolve search input debounce issue`).
- `chore:` For maintenance tasks (e.g., `chore: update dependencies`).
- `refactor:` For code restructuring (e.g., `refactor: improve API response handling`).
- `docs:` For documentation changes (e.g., `docs: update README with API details`).

## Version Control Strategy

The project follows **Semantic Versioning** (MAJOR.MINOR.PATCH):

- **MAJOR:** Breaking changes or overhauls.
- **MINOR:** New features that are backward compatible.
- **PATCH:** Bug fixes or small updates.

### Current Version: 1.0.0

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Edamam](https://developer.edamam.com/) for providing the Recipe Search API.
- Material-UI for React components.

## Author

- Jennifer James

