# 🚀 Kubernetes Elastic Infrastructure on AWS

This project implements a **Kubernetes infrastructure on AWS** designed to be **elastic, resilient, and automated**, using modern tools for **Infrastructure as Code (IaC), monitoring, and autoscaling**.  

The result is a highly available cluster that can automatically scale up or down depending on demand, optimizing **costs and performance**.

---

## 📌 Project Goals
- Deploy a managed Kubernetes cluster using **AWS EKS**.  
- Provision infrastructure with **Terraform** for reproducibility.  
- Implement **pod and node autoscaling**.  
- Enable **real-time monitoring and observability**.  
- Manage **external traffic** efficiently and securely.  

---

## 🏗️ Solution Architecture

- **Orchestration:** Kubernetes on Amazon EKS  
- **Infrastructure as Code:** Terraform to provision VPC, subnets, and EKS  
- **Metrics storage:** VictoriaMetrics (vmagent + victoria-metrics-single-server)  
- **Visualization:** Grafana dashboards  
- **Cluster observability:** kube-state-metrics + Metrics Server  
- **Autoscaling:**  
  - **HPA (Horizontal Pod Autoscaler):** scales pods automatically based on CPU/memory usage  
  - **Karpenter:** scales nodes dynamically to optimize performance and cost  
- **Traffic management:** Ingress-Nginx with subdomain routing and authentication  
- **Package management:** Helm for installation and upgrades of components  

---

## ⚙️ Services and Technologies Used
- AWS SSO Login  
- AWS EKS (Elastic Kubernetes Service)  
- AWS EBS  
- Terraform  
- Karpenter  
- VictoriaMetrics (vmagent and victoria-metrics-single-server)  
- Grafana  
- kube-state-metrics  
- Ingress-Nginx  
- Metrics Server  
- Horizontal Pod Autoscaler (HPA)  
- Helm  

---

## 🌍 Demo & Public Access
- 📊 **Grafana Public Dashboard:**  
  [View Dashboard](http://a6f28d2158180425ba5b05bebf33fc86-686528438.eu-west-1.elb.amazonaws.com:3000/public-dashboards/060a766092e34ad8a717fd4d2a12324c?from=now-12h&to=now&timezone=America%2FSantiago)  

- 🔥 **Stress Test Application:**  
  [Open Application](http://aws-kubernets-victoria-nginx-prometheus-karpenter-grafana-helm.danielweb.cl/)  

---
