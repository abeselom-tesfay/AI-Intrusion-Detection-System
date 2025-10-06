# Cloud-Based AI Intrusion Detection System for IoT Networks

## Project Overview
This project implements an **AI-powered intrusion detection system (IDS)** for IoT networks. It uses **Extreme Gradient Boosting (XGB)** and **deep learning techniques** to detect and classify various types of network attacks, ensuring the security and integrity of IoT environments.

## Dataset
The system leverages real-world IoT attack datasets, including:

- **MITM-ARPSpoofing**: Man-in-the-Middle attacks  
- **DoS-SYNFlooding**: Denial-of-Service attacks  
- **Scan-HostPort / Scan-PortOS**: Host and port scanning  
- **Mirai Malware Attacks**: UDP/ACK/HTTP flooding, Telnet brute-force  

All datasets are processed from **PCAP files**, transformed into tabular formats suitable for model training and evaluation.

## System Architecture
- **Data Pipeline**: Reads packet captures, preprocesses, labels, and generates feature sets.  
- **Model Training**: Trains XGB and LSTM-based models for anomaly detection and classification.  
- **Inference Pipeline**: Provides prediction on new IoT traffic and outputs analysis reports in CSV format.  
- **Real-Time Simulation**: Simulates live packet streaming for evaluation purposes.  

## Performance Metrics
- **F1 Macro Avg**: 0.997  
- **F1 Weighted Avg**: 1.0  
- **Inference Time per Data Point**: 1.07e-05 s  
- **Training Time**: 151.5 s  

The system demonstrates **high accuracy** and **real-world applicability** in detecting IoT network intrusions.
