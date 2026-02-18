# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [Do We Need More Training Data or Better
Models for Object Detection ?]

  - **[Link](https://www.bmva-archive.org.uk/bmvc/2012/BMVC/paper080/paper080.pdf)**
    
  - **Objective**:
    to determine whether object detection performance improves more from increasing training data size or from developing more complex and better-structured detection models.
  
  - **Methods**:
    The study evaluates HOG-based linear SVM object detectors by systematically varying training dataset size and model complexity (mixture components), using cross-validation and clean/supervised    clustering on large-scale datasets (PASCAL-10X and CMU MultiPIE).
  
  - **Outcomes**:
    Results show that more data can improve detection performance only with proper regularization and clean training data, but performance saturates quickly for standard mixture models,       while compositional part-based models (DPM/RMP) achieve significantly higher gains through parameter sharing and synthesizing unseen configurations
    
  - **Relation to the Project**:
  Our project relates to this study because both show that accurate predictions depend strongly on proper model tuning and regularization, since using more training data without adjusting      parameters can lead to overfitting and reduced performance.

- **Source 2**: [Comparative Review of Machine Learning Methods in Revenue 
Forecasting ]

  - **[Link](https://www.bmva-archive.org.uk/bmvc/2012/BMVC/paper080/paper080.pdf)**
    
  - **Objective**: The study aimed to accurately forecast the daily revenue of an e-commerce marketplace seller in order to support stronger financial planning.
    
  - **Methods**: The authors developed revenue forecasting models using Random Forest under three approaches: basic preprocessing, Isolation Forest outlier removal with mRMR feature selection, and DBSCAN clustering combined with feature selection before applying Random Forest.
    
  - **Outcomes**: The results showed that the DBSCAN clustering-based hybrid approach achieved the best forecasting accuracy, reducing the average error to 6.80% MAPE compared to 24.20% in the baseline approach.
    
  - **Relation to the Project**: The study shows that removing outliers improves prediction accuracy. Another learning is that instead of building one model for all days, they clustered the dataset and built a separate model for each cluster. This clustering of days improved the predictions highly. 

- **Source 3**: [Pre-Trained Language Models and Their Applications]

  - **[Link](https://doi.org/10.1016/j.eng.2022.04.024)**
  - **Objective**: The study aimed to provide a comprehensive review of pre-trained language models (PTMs) and explain their taxonomy, development, challenges, and real-world applications in natural language processing.
  - **Methods**: The authors conducted a structured literature review analyzing major PTM architectures (decoder-only, encoder-only, and encoder–decoder), scaling strategies, knowledge integration approaches, and downstream application areas
  - **Outcomes**: he study concluded that PTMs have transformed NLP through the pre-training and fine-tuning paradigm, enabling major performance gains across tasks, while highlighting key remaining challenges such as interpretability, robustness, reasoning ability, and deployment efficiency.
  - **Relation to the Project**: Our project is mainly a time-series forecasting / regression problem, while this study is about pre-trained language models (like BERT, GPT, T5) used for text understanding and generation. However, it becomes relevant if we inlcude text (for example google reviews, social media posts) into revenue prediction. 
