# NYC Airbnb Room Type Predictor

A simple Machine Learning web application that predicts Airbnb room types (*Entire home/apt, Private room, or Shared room*) in New York City based on listing features like price, location, and reviews.

## 🔗 Live Website
Check out the live deployment here: https://nyc-house-prediction-l.onrender.com/

## 🚀 How to Run Locally

### Using Docker (Recommended)
If you have Docker installed, you can pull and run the application with these two commands:

```bash
docker pull aahesan41/nyc-house-prediction:latest
docker run -p 8000:8000 aahesan41/nyc-house-prediction:latest
```
Once running, open your browser and go to: `http://localhost:8000`

### Without Docker
1. Activate your virtual environment and install requirements:
   ```bash
   pip install -r requirements.txt
   ```
2. Start the application:
   ```bash
   uvicorn main:app --host 127.0.0.1 --port 8000 --reload
   ```

## 🛠️ How Changes are Deployed
This project uses automated deployments. You do not need to push large images from your computer. 
Whenever you update your code and push it to GitHub, **GitHub Actions** automatically builds the Docker image and pushes it to Docker Hub, and **Render** pulls it to update the live website automatically.
