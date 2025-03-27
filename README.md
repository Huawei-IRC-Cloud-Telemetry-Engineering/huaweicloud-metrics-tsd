# Real or not? A Practitioner’s Perspective on Unsupervised Multivariate Time Series Anomaly Detection in Cloud Systems

Dataset Repository with 5 weeks of labeled timeseries for sock shop system with injected chaos disturbances. (under review KDD2025)

**Abstract:**

Anomaly detection in cloud infrastructure faces significant challenges due to the massive scale of data and complex interdependencies among metrics. While traditional research has primarily focused on single-metric detection, modern cloud systems require understanding relationships across multiple time series. The scarcity of labeled anomalies at scale makes supervised approaches impractical, creating a significant gap between academic solutions and industry requirements. In this work, we evaluate state-of-the-art unsupervised multivariate anomaly detection algorithms on established benchmarks and identify their practical limitations in real-world deployments. To bridge the research-practice gap, we introduce a comprehensive dataset comprising 74.5 million data points across 1311 metrics in multivariate time series. Our dataset can support multiple tasks other than anomaly detection like  forecasting, classification, explainability, and root cause analysis, serving both academic research and practical cloud monitoring needs. Through extensive empirical evaluation and practical insights, we demonstrate how theoretical approaches can be effectively adapted for production cloud environments.

**Dataset Folder Structure**

Dataset/
├── test/                  # Testing data (1 week)
│   ├── carts/             # Metrics for the carts service
│   │   ├── carts-2024-12-22-23.tar.gz
│   │   ├── carts-2024-12-23-00.tar.gz
│   │   └── ...
│   ├── catalogue/         # Metrics for the catalogue service
│   ├── ...                # Additional services
│   └── user/              # Metrics for the user service
│       ├── user-2024-12-22-23.tar.gz
│       ├── user-2024-12-23-00.tar.gz
│       └── ...
└── train/                 # Training data (4 weeks)
    ├── carts/             # Metrics for the carts service
    ├── catalogue/         # Metrics for the catalogue service
    ├── ...                # Additional services
    └── user/              # Metrics for the user service

Each service directory contains compressed files (`*.gz`) with hourly metric data. Files follow the format `service_name-` and contain CSV-formatted time series with timestamps and metric values.

**Limitation & Future Work**

1. Unknow Cascading Effect
2. Data Aggregation
3. Pointwise Evaluation
