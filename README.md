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

## How the Project Works
1. **Packet Sniffing:**

The tool starts by capturing network packets using a packet sniffer.
The captured packets are stored in a raw data file.
2. **Data Preprocessing:**

The raw data is preprocessed to extract relevant features needed for DDoS detection.
The preprocessed data is saved for further analysis.
3. **Machine Learning Model:**

The tool trains a machine learning model using historical network data.
The trained model is used to predict anomalies in the network traffic.
4. **Anomaly Detection:**

The tool analyzes the network traffic in real-time and uses the trained model to detect anomalies.
Anomalies are identified as potential DDoS attacks.
5. **IP Filtering**:

The tool checks and filters IP addresses based on predefined rules.
Suspicious IP addresses can be blacklisted to prevent further attacks.
6. **Visualization:**

The results of the detection are visualized to provide a clear understanding of the network traffic and detected anomalies.
Visualization helps in monitoring and taking preventive actions against DDoS attacks.

## Configuration and Usage

### Configuration
Clients can configure the tool using the `config.json` file, specifying paths for raw data, processed data, models, and logs.

### Usage
1. Clone the repository:
    ```bash
    git clone https://github.com/hibakhalidm/DDoS-detection-tool.git
    cd DDoS-detection-tool
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the main script:
    ```bash
    python src/main.py
    ```
