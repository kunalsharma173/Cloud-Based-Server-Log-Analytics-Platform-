# Cloud-Based-Server-Log-Analytics-Platform

## Overview
The Cloud-based Platform for Server Log Analytics is a powerful tool designed to parse, analyze, and visualize server log data, providing critical insights into website traffic, user behavior, and server performance. With real-time analytics and AWS Redshift integration, this platform enables data-driven decision-making for web administrators and businesses.

## Key Features
- **Log Parsing:** Extracts key metrics (visited URLs, user agents, referrers, etc.).
- **Traffic Analysis:** Identifies visitor trends, peak times, and navigation paths.
- **Device & Browser Detection:** Recognizes user demographics via browser and OS data.
- **Referrer Analysis:** Tracks search engines and external referral sources.
- **Comprehensive Reports:** Generates structured reports with visual charts.
- **Real-Time Insights:** Provides live monitoring of server activity.
- **AWS Redshift Integration:** Ensures scalable and secure log data storage.

## Installation & Setup
### 1. Install Python & Dependencies
Ensure Python is installed, then run:
```bash
pip install -r requirements.txt
```

### 2. Configure AWS Redshift
- Open inbound access to **port 5439**.
- Ensure outbound access for external communication.
- Update `/lib/redshift.py` with credentials:
```python
HOST = 'your-redshift-cluster-endpoint'
DATABASE = 'your-database-name'
USER = 'your-username'
PASSWORD = 'your-password'
PORT = '5439'
```

### 3. Run the Server
Navigate to the project directory and execute:
```bash
python main.py
```

### 4. Access the Dashboard
Open your browser and visit:
```bash
http://localhost:5000
```

## Usage
1. **Upload Logs:** Upload Apache, Nginx, or custom server log files.
2. **Analyze Data:** View traffic trends, user behavior, and performance insights.
3. **Generate Reports:** Export analytics reports in CSV or PDF formats.

## Security & Data Storage
- **AWS Redshift** ensures efficient storage and fast querying of large datasets.
- **Encryption** protects sensitive credentials and log data.

## Conclusion
This platform empowers web administrators and data analysts with actionable insights, optimizing website performance and user experience through intelligent log analytics.

---
Developed for scalable and secure server log analysis.

