# ✈️ FlightFinder - Flight Search and Notification System

## 📝 Project Overview
FlightFinder is a Python-based application that helps users find the cheapest flights from Mumbai (BOM) to multiple destination cities. It compares flight prices against the user's set budget and sends SMS notifications when a flight that fits the budget is found. 🤑💸

## 🚀 Features
- 📊 Loads destination city data and user budget information from an Excel sheet.
- 🌍 Automatically assigns IATA codes to destinations if missing.
- 🔍 Uses a flight API to search for the lowest-priced flights to each destination.
- 📲 Sends SMS notifications to users if a flight price is below their budget.
- 📋 Collects user details via a Google Form and stores them in a Google Sheet.
- 🎯 Personalized flight alerts based on user preferences.

## 📋 Requirements
- Python 3.x 🐍
- Libraries:
  - `requests` 🌐 for interacting with the flight API.
  - `twilio` 📱 for sending SMS notifications.
  - `google-api-python-client` 🗂️ for Google Sheets integration.

## ⚙️ Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/flightfinder.git

2. Install required dependencies:

   ```bash
   pip install -r requirements.txt

3. Set up API keys:
   - 🌍 Obtain API keys for the flight API (e.g., Amadeus API).
   - 📱 Set up your Twilio account to send SMS messages.
   - 📑 Create a Google API project and enable Google Sheets API for storing user details.
   - Update the `config.py` file with your API keys, Twilio credentials, and other necessary settings.

## 🏃‍♂️ Usage

1. Load your destination city and budget data into an Excel sheet. The sheet should contain columns for city name, IATA code (optional), and maximum budget.

2. Run the script to start the flight search and notification process:

   ```bash
   python flightfinder.py
   
3. The program will search for flights, compare prices with the user's budget, and send SMS alerts if a suitable flight is found.

## 📂 Files and Structure

- `flightfinder.py`: Main script to search for flights and send SMS notifications.
- `config.py`: Configuration file for storing API keys and credentials.
- `data.xlsx`: Sample Excel sheet with destination cities and budget info.
- `requirements.txt`: List of Python dependencies.

## 🤝 Contributing

Feel free to fork this repository and submit pull requests. If you have suggestions for improvements or encounter any bugs, please open an issue or contribute.

## 🙏 Acknowledgements

- ✈️ Thanks to Amadeus API for providing the flight data.
- 📱 Thanks to Twilio for the SMS API.
- 🗂️ Thanks to Google Sheets API for storing user preferences.
