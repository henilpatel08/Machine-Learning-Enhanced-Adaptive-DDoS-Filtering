In recent years, Distributed Denial-of-Service (DDoS) attacks have increased significantly in scale, frequency, and sophistication, posing serious risks to the stability and availability of global internet infrastructure. With recorded attack volumes exceeding 3.47 Tbps, conventional mitigation techniques—such as static filtering, IP blacklisting, and simple rate limiting—are no longer sufficient against modern, multi-vector, and highly dynamic attack patterns.

Although numerous adaptive filtering strategies have been proposed, including rule-generation methods like F-tree–based approaches, most existing research relies heavily on simulated datasets and assumes the availability of highly efficient detection systems. This assumption limits practical applicability in real-world network environments where detection latency, traffic diversity, and deployment constraints must be considered.

This project bridges the gap between theoretical DDoS filtering models and real-world operational deployment by introducing a machine learning–based adaptive DDoS filtering system. Rather than treating detection and mitigation as separate problems, we design an end-to-end pipeline that moves from raw traffic data ingestion to intelligent, dynamically generated filtering rules.

Our approach integrates:
- Real-time traffic classification using ensemble learning models
- Feature-driven rule construction for adaptive filtering
- Granularity-aware mitigation strategies that balance precision and network stability

We employ Random Forest and XGBoost classifiers trained on real-world network traffic datasets to accurately distinguish malicious from legitimate traffic. Beyond detection, we introduce a novel feature-driven granularity selection algorithm, which determines the most appropriate filtering scope (e.g., IP-level, port-level, subnet-level) based on feature importance and discriminative power. This ensures that mitigation actions are context-aware, minimizing collateral damage while maintaining high attack suppression effectiveness.

Unlike prior work that separates detection from mitigation, this system provides a cohesive pipeline that:
- Detects DDoS traffic using ensemble machine learning models
- Analyzes feature importance to guide filtering decisions
- Dynamically constructs adaptive filtering rules
- Deploys mitigation strategies aligned with best practices in model evaluation and operational feasibility

By tightly coupling intelligent detection with adaptive, feature-based rule generation, this project delivers a practical and scalable framework for modern DDoS defense suitable for real-world deployment environments.
