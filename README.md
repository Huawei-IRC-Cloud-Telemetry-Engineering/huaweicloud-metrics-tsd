# Fault Injected Anomaly Dataset (by Huawei Cloud)
The dataset was built for the purpose of anomaly detection and root cause anaysiss research work (by Ireland Research Center Huawei). The dataset consists of 5 weeks of labeled timeseries for [sock shop service](https://github.com/ocp-power-demos/sock-shop-demo) with injected chaos disturbances.

### Dataset Folder Structure

Dataset/<br>
├── test/ # Testing data (1 week) <br>
│ ├── carts/ # Metrics for the carts service <br>
│ │ ├── carts-2024-12-22-23.tar.gz <br>
│ │ ├── carts-2024-12-23-00.tar.gz <br>
│ │ └── ...<br>
│ ├── catalogue/ # Metrics for the catalogue service <br>
│ ├── ... # Additional services <br>
│ └── user/ # Metrics for the user service <br>
│ ├── user-2024-12-22-23.tar.gz <br>
│ ├── user-2024-12-23-00.tar.gz <br>
│ └── ...<br>
└── train/ # Training data (4 weeks)<br>
├── carts/ # Metrics for the carts service <br>
├── catalogue/ # Metrics for the catalogue service <br>
├── ... # Additional services <br>
└── user/ # Metrics for the user service <br>

Each service directory contains compressed files (`*.gz`) with hourly metric data. Files follow the format `service_name-` and contain CSV-formatted time series with timestamps and metric values.

### Limitation & Future Work
1. Unknow Cascading Effect
2. Data Aggregation
3. Pointwise Evaluation

### How to Use in Public Domain Publications and Articles
Even though the dataset is public and open-source under the Apache License (see License file), as a common courtesy, please update this README file by submitting a merge request and filling in the table in the "Publications and Usage" section below.

## Publications and Usage 

| No. | Year | Title | Abstract/Description |  Organization & Publication Info|
|-----|----- |-------|-------------|---------------|
| 1.  | 2025 | Real or not? A Practitioner’s Perspective on Unsupervised Multivariate Time Series Anomaly Detection in Cloud Systems | Anomaly detection in cloud infrastructure faces significant challenges due to the massive scale of data and complex interdependencies among metrics. While traditional research has primarily focused on single-metric detection, modern cloud systems require understanding relationships across multiple time series. The scarcity of labeled anomalies at scale makes supervised approaches impractical, creating a significant gap between academic solutions and industry requirements. In this work, we evaluate state-of-the-art unsupervised multivariate anomaly detection algorithms on established benchmarks and identify their practical limitations in real-world deployments. To bridge the research-practice gap, we introduce a comprehensive dataset comprising 74.5 million data points across 1311 metrics in multivariate time series. Our dataset can support multiple tasks other than anomaly detection like  forecasting, classification, explainability, and root cause analysis, serving both academic research and practical cloud monitoring needs. Through extensive empirical evaluation and practical insights, we demonstrate how theoretical approaches can be effectively adapted for production cloud environments. | Under Review |

## Other Data Contributions by Huawei
* Huawei Cloud's public and private serverless cloud platforms. ([See GitHub](https://github.com/sir-lab/data-release))
