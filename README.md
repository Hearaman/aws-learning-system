# ☁️ AWS Learning System - Amazon E-commerce Architecture

An interactive learning platform that teaches AWS services through a real-world Amazon-scale e-commerce example.

![AWS Learning System](https://img.shields.io/badge/AWS-Learning-orange)
![HTML5](https://img.shields.io/badge/HTML5-Dark-blue)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-green)

## 🎯 What is this?

This is a single-page, self-contained HTML application that explains **AWS services** using a **real Amazon-scale e-commerce architecture** as the example. Each service card shows:

- **What it does** in the Amazon architecture
- **Why Amazon chose it** for this use case
- **Real code/config examples** (Terraform, CLI, SQL, etc.)

## 🚀 How to use

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari)
2. Click on any service card to see details
3. Use the tabs (Compute, Storage, Database, etc.) to filter by layer
4. Explore the Amazon use case, purpose, reason, and example code for each service

## 📚 Services Covered

| Layer | Services |
|-------|----------|
| **Compute** | EC2, Auto Scaling Group, Lambda, ECS/EKS, Lightsail |
| **Storage** | S3, EBS, EFS, Glacier |
| **Database** | RDS, DynamoDB, ElastiCache, Aurora |
| **Network** | VPC, CloudFront, Route 53, ALB, API Gateway, Direct Connect |
| **Security** | IAM, KMS, WAF, Shield, GuardDuty |
| **Analytics** | Kinesis, Athena, QuickSight, Redshift |
| **Messaging** | SQS, SNS, EventBridge |

## 🏗️ Architecture Overview

```
Users → Route 53 → CloudFront/WAF/Shield → ALB → EC2/EKS/Lambda
                                                        ↓
                                  SQS/SNS/EventBridge → Aurora/RDS/DynamoDB/ElastiCache
                                                        ↓
                              Kinesis → S3/Glacier → Athena/Redshift/QuickSight
```

## 📖 Learning Features

- **Interactive Service Cards**: Click to explore each service in depth
- **Layer Filtering**: Focus on one architectural layer at a time
- **Real Code Examples**: Terraform, AWS CLI, SQL, YAML, JSON configurations
- **Amazon-Scale Context**: See how these services handle millions of users
- **Prime Day Scaling Story**: Understand how the architecture handles traffic spikes

## ⚡ Quick Start

```bash
# Clone the repository
git clone https://github.com/Hearaman/aws-learning-system.git

# Open in browser
open index.html  # macOS
# or just double-click index.html
```

## 📝 Note

This is a **learning architecture** illustrating common AWS patterns for a large Amazon-like commerce platform. It is **not** an official Amazon internal diagram.

## 🤝 Contributing

Feel free to add more services, improve descriptions, or enhance the UI. Just submit a PR!

## 📄 License

MIT License - Feel free to use and share!