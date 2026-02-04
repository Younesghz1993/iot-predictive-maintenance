# iot-predictive-maintenance
End-to-end Real-time IoT pipeline with Kafka, Spark Streaming, and ML.
# 🚂 End-to-End IoT Predictive Maintenance Pipeline

## 🚀 Overview
This project simulates a real-time IoT environment for Metro train compressors. It ingests high-frequency sensor data, processes it through a Medallion Architecture (Bronze/Silver/Gold) using **Spark Structured Streaming**, and applies a **Machine Learning** model to predict component failures.

## 🏗 Architecture
![Architecture Diagram](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/Apache_Spark_logo.svg/1200px-Apache_Spark_logo.svg.png)
*(Note: You can replace this with a diagram of your Kafka -> Spark -> ML flow later)*

### Tech Stack
* **Ingestion:** Apache Kafka (Producer/Consumer)
* **Processing:** Apache Spark Structured Streaming (PySpark)
* **Storage:** Data Lakehouse (Parquet format)
* **ML:** Spark MLlib (Random Forest Classifier)
* **Containerization:** Docker & Docker Compose

## 📂 Project Structure
* `docker-compose.yml`: Orchestrates Kafka, Zookeeper, Spark Master/Worker, and Jupyter Lab.
* `notebooks/Producer.ipynb`: Simulates IoT sensors by streaming CSV data to Kafka.
* `notebooks/Spark_Processor_*.ipynb`: ETL pipelines for Bronze (Raw), Silver (Cleaned), and Gold (Aggregated) layers.
* `notebooks/ML_Model_Training.ipynb`: Trains the Random Forest model on historical data.

## 🛠 How to Run
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/Younesghz1993/iot-predictive-maintenance.git](https://github.com/Younesghz1993/iot-predictive-maintenance.git)
2. **Start Services:**
```bash
  docker-compose up -d
```
3.**Access Jupyter Lab:** Go to http://localhost:8888 and run the notebooks in order:
  1.Producer
  2.Spark_Processor_Bronze
  3.Spark_Processor_Silver
  4.Spark_Processor_Gold

Results
Model Accuracy: 98.8%

Latency: Near real-time (<10 seconds)


---

### **Step 5: Push Code to GitHub**

Now, open your command prompt (CMD) or Git Bash in your project folder:

1.  **Initialize Git:**
    ```bash
    git init
    ```

2.  **Add your files:**
    ```bash
    git add .
    ```

3.  **Commit your changes:**
    ```bash
    git commit -m "Initial commit - Complete IoT Pipeline"
    ```

4.  **Link to GitHub (Copy the URL from the page you opened in Step 3):**
    ```bash
    git remote add origin https://github.com/Younesghz1993/iot-predictive-maintenance.git
    ```
   

5.  **Push the code:**
    ```bash
    git push -u origin main
    ```
    
