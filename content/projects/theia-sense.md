---
title: "Theia Sense"
date: 2025-06-01
draft: false
description: "AI-powered aesthetic image curation platform deployed on Azure Container Apps."
tags: ["Cloud", "ML", "Python"]
categories: ["Machine Learning", "Backend"]
showTableOfContents: true
showReadingTime: false
showDate: false
---

Full-stack, microservice-based application for aesthetic image curation. Features a decoupled FastAPI backend, a dedicated ML inference service, and a responsive frontend — deployed on Azure Container Apps and Hugging Face Spaces with independent auto-scaling.

**Project Link:** [theia.rutansh.dev](https://theia.rutansh.dev)

**GitHub:** [github.com/theia-sense/theia-sense](https://github.com/theia-sense/theia-sense)

**Languages:** Python

**Frameworks:** FastAPI, ONNX Runtime, Docker

**Infrastructure:** Azure Container Apps, Hugging Face Spaces

## Details

- An AI-powered curation model analyzes and scores user-uploaded images for aesthetic quality, using ONNX Runtime to reduce final container image size by 75% and improve inference speed
- A dynamic ranking algorithm adapts results to the collection's overall quality, providing a personalized user experience
- Deployed as microservices on Azure Container Apps, enabling independent scaling of FastAPI backend and ML inference service

<!-- ## Demo -->

<!-- Add a screenshot, gif, or video here -->
