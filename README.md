# Real or not? A Practitioner’s Perspective on Unsupervised Multivariate Time Series Anomaly Detection in Cloud Systems

Dataset Repository with 5 weeks of labeled timeseries for sock shop system with injected chaos disturbances. (under review KDD2025)

**Abstract:**

Anomaly detection in cloud infrastructure faces significant challenges due to the massive scale of data and complex interdependencies among metrics. While traditional research has primarily focused on single-metric detection, modern cloud systems require understanding relationships across multiple time series. The scarcity of labeled anomalies at scale makes supervised approaches impractical, creating a significant gap between academic solutions and industry requirements. In this work, we evaluate state-of-the-art unsupervised multivariate anomaly detection algorithms on established benchmarks and identify their practical limitations in real-world deployments. To bridge the research-practice gap, we introduce a comprehensive dataset comprising 74.5 million data points across 1311 metrics in multivariate time series. Our dataset can support multiple tasks other than anomaly detection like  forecasting, classification, explainability, and root cause analysis, serving both academic research and practical cloud monitoring needs. Through extensive empirical evaluation and practical insights, we demonstrate how theoretical approaches can be effectively adapted for production cloud environments.

**Dataset Folder Structure**

Dataset:
|───test
│   ├───carts
│   ├───catalogue
│   ├───coredns
│   ├───everest-csi-controller
│   ├───front-end
│   ├───istio-egressgateway
│   ├───istio-ingressgateway
│   ├───istiod
│   ├───kube-controller-proxy
│   ├───kube-state-metrics
│   ├───kubernetes
│   ├───locust-load-test
│   ├───log-agent-fluent-bit
│   ├───log-agent-otel-collector
│   ├───null-service
│   ├───orders
│   ├───orders-db
│   ├───payment
│   ├───queue-master
│   ├───rabbitmq
│   ├───shipping
│   └───user
└───train
    ├───carts
    ├───catalogue
    ├───coredns
    ├───everest-csi-controller
    ├───front-end
    ├───istio-egressgateway
    ├───istio-ingressgateway
    ├───istiod
    ├───kube-controller-proxy
    ├───kube-state-metrics
    ├───kubernetes
    ├───locust-load-test
    ├───log-agent-fluent-bit
    ├───log-agent-otel-collector
    ├───null-service
    ├───orders
    ├───orders-db
    ├───payment
    ├───queue-master
    ├───rabbitmq
    ├───shipping
    └───user

Each folder contains gz files showing hourly data collected for shown metrics.

**Limitation & Future Work**

1. Unknow Cascading Effect
2. Data Aggregation
3. Pointwise Evaluation
