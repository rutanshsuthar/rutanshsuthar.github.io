---
title: "StreamInsight"
date: 2026-01-15
draft: false
description: "Event-driven ML inference pipeline on AWS for scalable video analysis."
tags: ["MLOps", "AWS", "Python"]
categories: ["Machine Learning", "DevOps"]
showTableOfContents: true
showReadingTime: false
showDate: false
---

Scalable video analysis pipeline that processes uploaded videos through an event-driven architecture on AWS. An S3 upload triggers Lambda, which orchestrates Step Functions to coordinate Fargate containers and SageMaker Serverless inference, with results stored across two DynamoDB tables.

**GitHub:** [github.com/RutanshS/stream-insight](https://github.com/RutanshS/stream-insight)

**Languages:** Python, Bash

**Infrastructure:** AWS CDK, S3, Lambda, Step Functions, Batch (Fargate), SageMaker Serverless, DynamoDB

**ML:** OpenAI CLIP (ViT-B/32), PySceneDetect, FFmpeg

## How It Works

- S3 upload triggers Lambda → Step Functions orchestrate the full pipeline
- A containerized video processing job uses FFmpeg and PySceneDetect to extract keyframes at scene boundaries, dynamically scaling extraction volume with video duration to reduce downstream inference load by ~95%
- OpenAI CLIP (ViT-B/32) runs on SageMaker Serverless endpoints for zero-shot frame classification, with scale-to-zero to eliminate idle compute costs

<!-- ## Demo -->

<!-- Add a screenshot, gif, or video here -->
