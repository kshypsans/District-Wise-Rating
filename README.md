# Safety Index Prediction API

## Usage

1. Install dependencies:
   pip install -r requirements.txt

2. Start the Flask server:
   python app.py

3. Send a POST request to the `/predict` endpoint with the following JSON payload:
   {
       "latitude": 28.7041,
       "longitude": 77.1025
   }

   example usage:
   curl -X POST http://127.0.0.1:5000/predict \
    -H "Content-Type: application/json" \
    -d '{"latitude": 28.7041, "longitude": 77.1025}'

4. Example Response:
    json
   {
       "district": "North Delhi",
       "state": "Delhi",
       "year": 2025,
       "safety_index": 0.78
   }

