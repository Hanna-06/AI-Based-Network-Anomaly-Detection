# AI-Based-Network-Anomaly-Detection
 This project focuses on real-time network traffic monitoring and anomaly detection using an Isolation Forest model. The system captures network packets, extracts relevant features such as bytes sent, bytes received, and connection counts and logs them in a structured dataset. The Isolation Forest algorithm is trained to identify anomalous behavior in the network traffic, categorizing packets as normal (1) or suspected anomalies (-1). The processed data is then visualized through a Flask-based web dashboard, providing an intuitive interface for users to monitor network activity and anomaly trends. The project integrates automated packet capture, periodic model retraining, and interactive data visualization using Plotly to enhance network security insights. By detecting suspicious IP activities in real time, this system serves as a proactive defense mechanism against potential cyber threats. The combination of machine learning, real-time processing, and web based visualization makes it a valuable tool for cybersecurity applications.

DIRECTORY STRUCTURE:

AI-Based Network Anomaly Detection/
|
|-------app/
|     |-------templates/
|     |     |-------dashboard.html
|     |-------__init__.py
|     |-------main.py
|     |-------model.py
|     |-------packet_capture.py
|     |-------utils.py
|-------data/
|     |-------network_logs.csv                     <-----captured packet details
|     |-------network_logs_with_anomalies.csv      <-----output file with anomaly scores
|-------models/
|     |-------isolation_forest_model.pkl           <-----trained model
|-------run.py
