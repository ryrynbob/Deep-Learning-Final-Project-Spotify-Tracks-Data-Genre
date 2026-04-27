# Deep-Learning-Final-Project-Spotify-Tracks-Data-Genre




## Decoding Music DNA: Multi-Label Genre Affinity
## Course: MSDS 6393 A - Deep Learning (Spring 2026)
## Professor: Dr. Lukas Simon
## Author: Ryan Nguyen

## Quick Access:
Because of the extensive data mapping and high-resolution visualizations, the primary notebook may be too large for GitHub's native preview. Please use the link below to view the interactive results, training curves, and the Music DNA tool:

## Project Overview:
This project moves beyond traditional "one-box" genre classification. By analyzing 114,000 Spotify tracks, I developed a deep learning framework that treats musical genre as a spectrum of affinities—Music DNA—rather than a mutually exclusive category.
## Key Technical Achievements:
The Pivot to Sigmoid: Switched from Softmax to Sigmoid activation to allow for "Crossover" genre detection (e.g., a song that is 80% Electronic and 40% Pop). 
Binary Focal Loss: Implemented Focal Loss ($\gamma = 2.0$) to force the model to learn rare genres (Hip-Hop, Classical) instead of over-predicting the majority "Indie" class.
Dynamic Thresholding: Optimized classification cutoffs per genre to maximize the Macro F1-score, moving past the blunt $0.5$ default.
Unsupervised Reality Check: Built an Autoencoder with a 4D bottleneck to prove that audio features naturally overlap, justifying the multi-label approach.

## 📊 Key Results & Visualizations:

The hidden gem discovery: Found that "Hark The Herald Angels Sing" (Rock) shares a 99.9% Acoustic Similarity with J-Pop tracks, proving that audio structure transcends cultural labels.
SHAP Interpretability: Documented exactly which "Genotypes" (Acousticness, Energy, etc.) the model uses to make its decisions.
Training Stability: Demonstrated a simulated 7-day deployment with steady performance, proving the model generalizes well to new data.

## 🛠️ Repository Structure

FinalProject_SpotifyTracks_Ryan_REALDEAL: The core interactive Jupyter Notebook.

README.md: Project documentation and executive summary.

Canva Report: Technical Blog Style Report

Presentation: Capstone Slides
