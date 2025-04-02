# Stock Tracker

A modern React application for tracking stock market data and maintaining a personal watchlist of your favorite stocks.

## Features

- **Real-time Stock Data**: View current prices and percentage changes for stocks
- **Market Cap Information**: See market capitalization data for companies
- **Search Functionality**: Search for stocks by company name or symbol
- **Persistent Watchlist**: Save your favorite stocks to a watchlist that persists between sessions

## Demo

[View Live Demo](#) <!-- Add your deployment link when available -->

## Technology Stack

- **Frontend**: React, React Router, Context API
- **API**: Finnhub Stock API
- **Storage**: Local Storage for watchlist persistence
- **Styling**: Custom CSS

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/stock-tracker.git
   cd stock-tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your Finnhub API key:
   ```
   REACT_APP_FINNHUB_API_KEY=your_api_key_here
   ```

4. Start the development server:
   ```bash
   npm start
   ```

## Usage

### Home Page
The home page displays the top stocks by market capitalization. You can search for specific stocks using the search bar at the top of the page.

### Watchlist
Click the star icon on any stock card to add it to your watchlist. Visit the Watchlist page to view all your saved stocks. The watchlist is saved in your browser's local storage and will persist even if you close the browser.

### Stock Information
Each stock card displays:
- Company name and symbol
- Current stock price
- Percentage change
- Market capitalization

## Project Structure

```
stock-tracker/
├── public/
├── src/
│   ├── components/         # Reusable UI components
│   │   ├── NavBar.jsx      # Navigation bar component
│   │   └── StockCard.jsx   # Individual stock display component
│   ├── contexts/
│   │   └── StockContext.jsx # Global state management
│   ├── css/                # CSS styles
│   ├── pages/
│   │   ├── Home.jsx        # Home page with search and trending stocks
│   │   └── Watchlist.jsx   # User's saved stocks
│   ├── services/
│   │   └── api.js          # API service functions
│   ├── App.jsx             # Main application component
│   └── main.jsx            # Entry point
└── package.json
```

## API Integration

This application uses the [Finnhub Stock API](https://finnhub.io/) to fetch stock data. The integration includes:

- Getting top stocks by market cap
- Searching for stocks by name or symbol
- Fetching detailed stock information including price, change percentage, and company profiles

## Future Enhancements

- Historical price charts
- News feed for each stock
- Portfolio tracking with performance metrics
- Additional technical indicators
- Dark mode support

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Finnhub](https://finnhub.io/) for providing the stock market data API
- [React](https://reactjs.org/) and [React Router](https://reactrouter.com/) for the frontend framework
- All contributors and testers who helped improve this application
