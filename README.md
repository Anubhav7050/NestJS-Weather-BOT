**Weather Bot Telegram - Nest.js**
Weather Bot Telegram is a sophisticated and user-friendly Telegram bot built using Nest.js, designed to provide real-time weather updates and forecasts to users. The bot allows users to subscribe to weather notifications for specific cities, keeping them informed with the latest weather information directly in their Telegram app.

Whether you’re planning your day or keeping track of changing weather patterns, this bot ensures that users are always up-to-date with weather forecasts tailored to their chosen locations.

![Screenshot (147)](https://github.com/user-attachments/assets/8e9851e8-5ff9-4f58-908e-872fdd2d45a3)

**Table of Contents**
Features
Prerequisites
Installation
Configuration
Usage
Commands
Endpoints
Contributing
License

**Features**
**Real-time weather updates**: Receive the latest weather data for any subscribed city.
**Subscription management**: Users can easily subscribe and unsubscribe to weather updates for specific locations.
**MongoDB integration**: User data, including subscriptions, are stored in MongoDB.
**Seamless Telegram interaction**: Users can interact with the bot through simple Telegram commands like /subscribe and /unsubscribe.
**OpenWeatherMap integration**: Fetch accurate and detailed weather information using the OpenWeatherMap API.
**Customizable alerts**: Set up periodic weather updates to keep users informed.

**Prerequisites**
Before you begin, ensure that the following tools are installed:

**Node.js** (version 16.x or later recommended)
**MongoDB** (for storing user and subscription data)
**npm or yarn**

**Installation**
**1. Clone the repository**
git clone https://github.com/yourusername/weather-bot-telegram.git

**2. Navigate to the project folder**
cd weather-bot-telegram

**3. Install project dependencies**
npm install

Or, if you prefer Yarn:
yarn install

**4. Configure the environment variables**
In the root directory of the project, create a .env file and configure the following environment variables:
TELEGRAM_BOT_TOKEN=YOUR_TELEGRAM_BOT_TOKEN
MONGODB_URI=YOUR_MONGODB_CONNECTION_URI
OPENWEATHERMAP_API_KEY=YOUR_OPENWEATHERMAP_API_KEY
CITY=YOUR_DEFAULT_CITY (Optional, set a default city for the bot to track)

**TELEGRAM_BOT_TOKEN**: Your unique token from BotFather.
**MONGODB_URI**: The connection string for your MongoDB database.
**OPENWEATHERMAP_API_KEY**: Your API key from OpenWeatherMap.
**CITY**: Default city for weather tracking (optional).

**5. Start the bot**
To start the bot, run the following command:
npm run start

Your Weather Bot is now live and ready to serve weather updates via Telegram!

**Usage**
Once the bot is running, users can interact with it by sending commands to receive real-time weather updates.

**Commands**
**/subscribe [city]**: Subscribe to receive weather updates for the specified city.
**/unsubscribe**: Unsubscribe from weather updates.
**/status**: Get the current weather for your subscribed city.
**/help**: Display a list of available commands.
Users can subscribe to as many cities as they wish and will receive periodic weather updates based on their preferences.

**Endpoints**
The Weather Bot exposes the following endpoints for handling user requests:

**/subscribe**: Allows users to subscribe to weather updates for a specific city.
**/unsubscribe**: Unsubscribes the user from all weather notifications.
**/status**: Provides the current weather details of the subscribed city.
These endpoints handle communication between the Telegram bot and the back-end server to send notifications.

**Contributing**
We welcome contributions to Weather Bot Telegram! If you’d like to contribute, please follow these guidelines:

Fork the repository.
Create a new branch: git checkout -b feature/your-feature.
Implement your changes.
Write tests (if applicable).
Commit your changes: git commit -m 'Add new feature'.
Push to your branch: git push origin feature/your-feature.
Open a pull request.

**Code of Conduct**
Please make sure to follow the project’s code of conduct when contributing. Be respectful and considerate in your interactions with the community.

**License**
This project is licensed under the MIT License. Feel free to modify, distribute, and contribute according to the open-source guidelines.

**Additional Information**

Weather Bot Telegram was built with ease of use in mind. The modular and extensible architecture of Nest.js ensures that this bot can be easily maintained, extended, and scaled in the future. Whether you're interested in contributing, customizing the bot for your own use case, or simply looking for a weather notification system, this project provides a solid foundation.
