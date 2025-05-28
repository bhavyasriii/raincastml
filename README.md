RainCastML - Real-Time Rain Prediction App

RainCastML is a web application that predicts whether it will rain in a given city using real-time weather data from the OpenWeatherMap API and a machine learning model (Random Forest Classifier). Built with Python and Streamlit.

Features:
- Real-time weather input by city name
- Machine learning prediction (Rain or No Rain)
- Displays temperature, humidity, pressure, wind speed, cloud cover, and description
- Dynamic and clean user interface using Streamlit
- Secure API key management using .env or Streamlit Cloud Secrets

Project Structure:
- app.py              → Streamlit frontend application
- train_model.py      → Script to train the ML model
- raincast_model.pkl  → Saved trained model
- requirements.txt    → Python dependencies
- .env                → Local environment variable file (not pushed to GitHub)
- README.md           → Project overview and instructions

How to Run Locally:
1. Clone the repo:
   git clone https://github.com/yourusername/raincastml.git
   cd raincastml

2. Install dependencies:
   pip install -r requirements.txt

3. Add your API key:
   Create a file called `.env` in the root folder and add this line:
   OPENWEATHERMAP_API_KEY=your_actual_api_key

4. Run the app:
   streamlit run app.py

Deployment Instructions (Streamlit Cloud):
1. Push the project to GitHub.
2. Go to streamlit.io/cloud and link your GitHub repo.
3. Set `app.py` as the main file.
4. In Settings > Secrets, add:
   OPENWEATHERMAP_API_KEY = your_actual_api_key
5. Deploy and share your live app URL.

Author:
Bhavyasri Mudireddy

License:
MIT License – free to use, modify, and learn.
