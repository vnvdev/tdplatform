# Xcule

![Xcule Logo](client/src/logo.png)

Xcule is a revolutionary trading analysis tool designed for every trader out there! Whether you're into SMC or ICT trading, Xcule has got you covered. Dive deep into the world of technical analysis with our advanced features tailored to visualize Institutional Trading Strategies.

## Features

- **Trading Analysis Tool:** Designed specifically for SMC (Smart Money Concepts) traders.
- **Real-time Market Data:** Integrated with real-time market data for up-to-date analysis.
- **Multiple Chart Views:** Supports multiple chart views for comprehensive analysis.
- **Easy Drawing of Market Structures:** Allows users to easily draw market structures, Points of Control (POS), demand and supply zones.
- **Remove Unwanted Drawings:** Ability to remove unwanted drawings from the object tree.
- **SMC Drawing Across Time Frames:** Draw SMC structures for all time frames inside one chart.
- **Combine SMC Drawings:** Draw SMC structures at different time frames (e.g., 30 minutes and 15 minutes) into one-hour charts.
- **Fair Value Gaps (FVG):** Draw fair value gaps of any time frame and view them inside one-hour charts.
- **Lower Time Frame Analysis:** Analyze fair value gaps and manipulations in lower time frames like 5 minutes, 3 minutes, and 1 minute.
- **Manipulation Drawing:** Draw market manipulations for different time frames (e.g., one-minute manipulations inside one-hour charts).
- **Replay Mode for Strategy Testing:** Test trading strategies using replay mode, even in smaller time frames like 5 minutes, 3 minutes, and 1 minute.
- **Comprehensive Tool:** All features are integrated into one comprehensive tool for seamless analysis.

## Demo

[![Xcule Features Video](https://img.youtube.com/vi/oFk-KcKAiCI/0.jpg)](https://www.youtube.com/watch?v=oFk-KcKAiCI)

## Getting Started

### Prerequisites

- Docker
- Docker Compose

### Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/yourusername/xcule.git
   cd xcule
   ```

2. **Create a `.env` file:**

   Create a `.env` file in the root directory with the following content:

   ```env
   MONGODB_USER=your_mongo_user
   MONGODB_PASSWORD=your_mongo_password
   MONGO_DB_HOST=your_mongo_host
   MONGODB_DOCKER_PORT=27017
   MONGO_DB_SERVER=mongodb
   MONGO_DB_NAME=your_db_name
   EXPRESS_PORT=3000
   EXPRESS_SOCKET_PORT=3001
   FLASK_PORT=5000
   FLASK_HOST=0.0.0.0
   MONGO_EXPRESS_PORT=8081
   MONGO_EXPRESS_USER=your_express_user
   MONGO_EXPRESS_PASSWORD=your_express_password
   ```

3. **Build and run the services:**

   ```sh
   docker-compose up --build
   ```

### Services

- **Node.js Service:** Fetches real-time indicator data from TradingView charts.
- **Flask Service:** Loads Smart Money Concepts (SMC) information such as Market Structure, Supply & Demand zones, Imbalance Zones, etc.
- **MongoDB Service:** Stores trading data.
- **Mongo Express Service:** Provides a web-based interface for MongoDB.

## Usage

1. **Access the Node.js API:**

   Open your browser and go to `http://localhost:3000`.

2. **Access the Flask API:**

   Open your browser and go to `http://localhost:5000`.

3. **Access Mongo Express:**

   Open your browser and go to `http://localhost:8081`.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Ryan Saleh - [@ryansaleh](https://www.linkedin.com/in/ryan-saleh-84b73885/) - hello@ryansaleh.com

Project Link: [https://github.com/MohdSaleh/xcule](https://github.com/MohdSaleh/xcule)

## Acknowledgements

- [TradingView](https://www.tradingview.com/)
- [Docker](https://www.docker.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongo Express](https://github.com/mongo-express/mongo-express)

---

Made with ❤️ by [Ryan Saleh](https://github.com/MohdSaleh)
```

### Notes

- Replace placeholders like `yourusername`, `your_mongo_user`, `your_mongo_password`, etc., with actual values.
- Customize the contact information and acknowledgments as needed.
