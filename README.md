# DDoS Detection Tool

This project is designed to detect Distributed Denial of Service (DDoS) attacks using various machine learning algorithms. The tool captures network packets, processes the data, applies machine learning models, and visualizes the results.

## Features
- Real-time packet capture
- Feature extraction from network packets
- Machine learning-based DDoS detection
- Visualization of network traffic
## Directory Structure

- `src/`: Source code
  - `main.py`: Main script
  - `preprocess.py`: Data preprocessing
  - `utils/config.py`: Configuration
- `data/`: Data storage
  - `raw/captured_traffic.csv`: Raw captured traffic
  - `processed/`: Processed data
  - `anomalies/`: Anomalies data
- `models/`: Trained models
- `logs/`: Log files

## Configuration Paths

- `RAW_DATA_PATH`: Path to raw captured traffic (`data/raw/captured_traffic.csv`)
- `PROCESSED_DATA_PATH`: Path to processed data (`data/processed/processed_data.csv`)
- `MODEL_PATH`: Path to trained model (`models/ddos_model.pkl`)
- `ANOMALY_DATA_PATH`: Path to anomaly data (`data/anomalies/anomaly_data.csv`)
- `LOG_PATH`: Path to log file (`logs/app.log`)
- `THRESHOLD_PACKET_RATE`: Packet rate threshold for detection (example: 100)
## Requirements

The following Python packages are required to run this project:
- scapy
- pandas
- numpy
- scikit-learn
- joblib
- matplotlib
- logzero
- datetime

You can install them using the following command:
```bash
pip install -r requirements.txt
```

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/hibakhalidm/DDoS-detection-tool.git
    cd DDoS-detection-tool
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Run the main Python script:
    ```bash
    python src/main.py
    ```


