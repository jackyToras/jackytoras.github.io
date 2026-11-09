---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 2
---
<style>
.project-row {
  display: flex;
  border-top: 1px solid #ddd;
  padding: 20px 0;
}
.project-content { flex: 1; }
.project-content h4 { font-weight: 700; margin-bottom: 4px; }
.project-content .tech { font-size: 0.85rem; color: gray; margin-bottom: 8px; }
.project-content .links { margin-bottom: 8px; }
.project-content .links a { margin-right: 10px; }
</style>
<div class="project-row">
<div class="project-content">
<h4>Distributed Task Queue System</h4>
<div class="tech">Java · Spring Boot · RabbitMQ · Docker · AmazonEC2</div>
<div class="links"><a href="https://github.com/jackyToras/Distributed-tasks-queue-system" target="_blank">GitHub</a> <a href="http://3.109.219.82:15672" target="_blank">Live</a></div>
Architected a high-throughput, distributed message queue designed to process heavy background workloads asynchronously without blocking the main application thread. Utilized a competing consumers pattern across multiple parallel worker nodes to ensure high availability and eliminate single points of failure. Engineered reliability into the pipeline by persisting tasks to a PostgreSQL database for durable storage and configuring RabbitMQ prefetch counts to prevent worker overload. Implemented automated fault handling by routing failed tasks to a Dead Letter Queue equipped with customizable retry logic.
</div>
</div>
<div class="project-row">
<div class="project-content">
<h4>Scalable Microservices Salon Booking Platform</h4>
<div class="tech">Spring Boot · RabbitMQ · React.js · MongoDB · API Gateway · Stripe · Keycloak · Docker</div>
<div class="links"><a href="https://github.com/jackyToras/salon-appointment-system" target="_blank">GitHub</a></div>
Architected an production-grade, 9-service ecosystem featuring decoupled business domains for bookings, payments, and notifications. Configured a Spring Cloud Gateway to route traffic dynamically using Eureka service discovery while securing endpoints via Keycloak JWT authentication. Implemented asynchronous, event-driven communication using RabbitMQ to process background transactions without blocking core operations. Orchestrated the entire infrastructure using Docker Compose with strict health-check dependencies to ensure a fault-tolerant container startup sequence.
</div>
</div>
<div class="project-row">
<div class="project-content">
<h4>askPDF</h4>
<div class="tech">FastAPI · LangChain · ChromaDB · Ollama · Python · React.js · Tailwind CSS</div>
<div class="links"><a href="https://github.com/jackyToras/askPDF" target="_blank">GitHub</a></div>
Built a retrieval-augmented generation (RAG) app for PDF and DOCX question answering. The FastAPI and LangChain pipeline splits documents into 500-character chunks with 50-character overlap, stores embeddings in ChromaDB, and retrieves the top five results by cosine similarity. A local Ollama LLM generates context-grounded answers. Per-user data isolation and persistent chat history scope uploads and conversations to user IDs. The React and Tailwind CSS interface includes Markdown rendering and a timeout-aware REST client.
</div>
</div>
<div class="project-row">
<div class="project-content">
<h4>Cyber AI Network Intrusion Detection System</h4>
<div class="tech">Python · Scikit-learn · Pandas · NumPy · Streamlit</div>
<div class="links"><a href="https://github.com/jackyToras/NetworkIDS" target="_blank">GitHub</a> <a href="https://mlnetworkids.streamlit.app" target="_blank">Live</a></div>
An ML based network intrusion detection pipeline analyzing network traffic features to classify flows as benign or malicious with 96.4% accuracy. Trained on the CICIDS benchmark dataset, the system processes network flow characteristics—derived from packet capture (.pcap) or csv files—to detect major attack vectors including DoS/DDoS, Port Scans, Brute Force, and Botnets. Built using a robust Random Forest ensemble model with stratified sampling to counter inherent network class imbalances, the pipeline features a Streamlit dashboard visualizing feature importance scoring for transparent model inference.
</div>
</div>
