
 # Fashion Recommender System: Optimizing Fashion Recommendations for Diverse Body Types

## Overview

This project introduces a novel recommendation system for fashion e-commerce platforms that caters to users with diverse body types. It uses a dual-layer model architecture incorporating both content-based filtering and a reinforcement learning-based approach utilizing the Epsilon Greedy algorithm. The goal is to provide personalized fashion recommendations based on user-specific body measurements or photograph analysis.

### Key Features:
- **Body Type Identification**: Utilizes both manual measurements and photographic analysis to identify user body types (hourglass, pear, apple, inverted triangle, rectangle).
- **Content-Based Filtering**: Generates personalized recommendations by aligning clothing characteristics (e.g., occasion, gender) with user preferences.
- **Reinforcement Learning (Epsilon Greedy)**: Adapts recommendations dynamically by balancing exploration of new items and exploitation of user-preferred choices.
- **Clustering Layer**: Provides an initial set of recommendations based on user input.
- **Reinforcement Layer**: Continuously refines recommendations based on user interactions and feedback.
- **High Engagement Metrics**: Achieves a click-through rate of 46% and a novelty score of 84%.
## System Architecture

The system is divided into two main layers:

1. **Clustering Layer**: Uses content-based filtering to generate initial recommendations based on user-provided body type and preferences.
2. **Reinforcement Layer**: Implements the Epsilon Greedy algorithm to adapt recommendations based on user interaction, balancing between exploring new options and reinforcing previously liked items.
![Top K Recommendations](https://github.com/user-attachments/assets/78a2abb4-b720-4332-9537-ace34b2c4874)
## Dataset

- **Clothing Dataset**: The dataset contains 8,000 images of clothing items scraped from various e-commerce platforms. Each item is annotated with metadata, including body type, occasion, and gender.
- Preprocessing is done using the **ResNet50** model to extract high-level visual features, which are stored in a SQLite database for efficient retrieval.

## Evaluation

The model was evaluated on several key metrics:
- **Click-Through Rate (CTR)**: 46% 
- **Novelty Score**: 84%
- **Exploration-Exploitation Tradeoff**: 62% exploration, 38% exploitation

These metrics demonstrate the system's ability to provide both familiar and new recommendations, resulting in high user engagement.




