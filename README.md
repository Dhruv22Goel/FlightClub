# ✈️ Flight Deal Finder

A Python project that searches for cheap flights and sends you notifications when deals are found.  

## 📌 Features
- Search for the cheapest flights using an API.  
- Store and manage flight data in Google Sheets (or a local database).  
- Get notified via SMS/Email when flight prices drop.  
- Configurable departure city and destination list.  

## 📂 Project Structure
```
├── main.py                # Entry point of the app
├── data_manager.py        # Handles reading/writing data (e.g., Google Sheets API)
├── flight_data.py         # Defines FlightData class for storing flight info
├── flight_search.py       # Handles API requests to search flights
├── notification_manager.py # Sends notifications (SMS/Email/Telegram)
```

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/flight-deal-finder.git
cd flight-deal-finder
```

### 2. Install dependencies
Make sure you have Python 3.10+ installed. Install required packages:
```bash
pip install -r requirements.txt
```

### 3. Set up environment variables
Create a `.env` file in the root directory with your API keys and credentials:
```
TEQUILA_API_KEY=your_api_key
SHEETY_API_URL=your_sheety_url
SHEETY_API_TOKEN=your_sheety_token
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE=your_twilio_number
MY_PHONE=your_verified_phone
```

### 4. Run the project
```bash
python main.py
```

## 🔔 Notifications
Currently supports:
- **SMS (Twilio)**
- (Optional) Email / Telegram  

You’ll receive alerts like:  
```
Low price alert! Only $250 to fly from New York to Paris, 12 Mar - 20 Mar.
```

## 🛠️ Tech Stack
- **Python**  
- **Requests** (API calls)  
- **Twilio** (SMS notifications)  
- **Sheety / Google Sheets API** (data storage)  

## 📌 Future Improvements
- Add support for multiple departure cities  
- Integrate Telegram bot notifications  
- Automatic scheduling (cron/Task Scheduler)  
