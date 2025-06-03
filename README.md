# MSHA Dermatology Diagnostic Model Deployment

## Project Summary
Deployed a Dockerized deep learning model for diagnosing skin lesions using Multi-Scale Hierarchical Attention (MSHA) architecture. Hosted on AWS via Flask API, it reduced dermatologist review time by 60%.

## Problem Statement
Manual dermatological diagnosis was time-consuming and inconsistent. A clinically deployable tool was needed to assist dermatologists by automating the classification of skin lesions.

## Tools & Technologies Used
- **ML Model**: MSHA (Multi-Scale Hierarchical Attention Network)  
- **Deployment**: Flask API, Docker, AWS EC2  
- **Languages**: Python (PyTorch, OpenCV)  
- **Data**: Dermoscopic images (HAM10000, internal annotated datasets)

## Approach
- Trained MSHA CNN to capture hierarchical features in lesion images  
- Evaluated model on classification accuracy, sensitivity, and F1-score  
- Containerized the solution using Docker and deployed it to AWS EC2  
- Built a clinician-facing web interface for image upload and diagnosis output

## Deployment Pipeline
```
User Upload ─▶ Flask API ─▶ Dockerized MSHA Model ─▶ Diagnosis Output ─▶ Clinician
```

## Results & Clinical Impact
- 60% reduction in dermatologist review time  
- High-accuracy model assisted in triaging benign vs malignant lesions  
- Improved consistency and early detection rates across departments

## Monitoring & Maintenance
- API endpoints monitored for uptime and latency  
- Manual review feedback loop integrated for retraining with real-world data

## Challenges & Learnings
- Ensured inference speed under 500ms with GPU-optimized containers  
- Managed class imbalance with augmented training data  
- UI/UX simplicity was crucial for clinical adoption

## Team Collaboration
- Collaborated with dermatologists and software engineers  
- Delivered training to medical staff on system usage

## Code Availability
Source code and image data are proprietary and cannot be publicly shared.
