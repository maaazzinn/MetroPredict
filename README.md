# Project Name: MetroPredict: Smart Ridership Forecasting for Kochi Metro

## Description

MetroPredict is a metro crowd prediction and analysis system that uses computer vision and deep learning to analyze crowd density at metro stations based on video input. It consists of a Flask-based backend, a YOLOv8 object detection model, and a web interface built with HTML, CSS, and JavaScript to visualize results.

## Project Overview

This mini project processes video footage from metro stations to estimate and analyze crowd density. The system integrates a YOLOv8 deep learning model with a Flask-based API and a frontend visualization tool.

## How It Works

### Video Processing

- The project processes videos from metro stations using YOLOv8 to detect people and estimate crowd density.
- The system uses pre-recorded footage from stations like **Aluva, Edappally, Kalamassery, Lissie, and MG Road**.
- Currently, **dummy videos** of crowd scenarios are provided in the `data/videos/` folder.
- Future improvements will include the integration of **live CCTV footage** for real-time crowd tracking.

### Backend Functionality (Flask API)

- Handles video input and processes crowd analysis.
- Reads metro station details from `metro_stations.json`.
- Stores crowd estimation results in `crowd_data.json`.

### Frontend (Web Interface)

- Developed using **HTML, CSS, and JavaScript**.
- Displays crowd predictions for different stations.
- Allows users to visualize real-time or past crowd density.

## Expected Outcomes

- Real-time or historical crowd density predictions for metro stations.
- Visual representation of crowd levels for better decision-making.
- A working prototype showcasing AI-based metro station analysis.
- Future capability to process **live CCTV feeds** for real-time updates.

## Project Structure

- **frontend/** - Contains the frontend code, built with HTML, CSS, and JavaScript.
- **backend/** - Contains the backend logic, built using Flask and YOLOv8 for object detection.
- **data/** - Stores relevant datasets, including metro station details and crowd density estimations.
- **data/videos/** - Contains **dummy crowd videos**, which can be replaced with live CCTV footage in future implementations.
- **main.py** - The main entry point of the application.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/maaazzinn/MetroPredict
   cd MetroPredict
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Navigate to the backend directory and start the backend server:
   ```sh
   cd backend
   python app.py
   ```
4. Navigate to the frontend directory and start the frontend server:
   ```sh
   cd frontend
   Open index.html in a web browser.
   ```

## Usage

- Open the `index.html` file in a web browser after the backend is running.
- Interact with the interface to see crowd predictions for metro stations.
- Modify the `data/videos/` folder to replace dummy videos with actual CCTV footage when implementing real-time tracking.

## Contributing

Feel free to fork this repository, submit pull requests, or suggest improvements.

## License

This project is licensed under the MIT License.

