# Data Source
- Protein sequences were downloaded from UniProtKB (https://www.uniprot.org/).  
- Two groups:
Normal conditions: 100 proteins
Drought stress: 100 proteins
# Comparing Normal and Drought-Stressed Proteins
Proteins under normal conditions and under drought stress were analysed to reveal amino acid patterns and sequence features linked to drought response.  
Normal proteins: control/baseline  
Drought-stressed proteins: stress response  
This allows a machine learning model to distinguish between baseline and stress-responsive proteins.
# Methods
1. Feature Extraction
   - Amino acid composition: frequency of each of the 20 standard amino acids.
2. Machine Learning
   - Random Forest classifier (scikit-learn) used for binary classification.
   - Train/Test split: 80/20
   - Hyperparameter tuning: GridSearchCV for `n_estimators`, `max_depth`, `min_samples_split`
3. Evaluation
   - Accuracy and confusion matrix.
   - Feature importance to identify amino acids most relevant to drought response.
# Results
- The model highlighted amino acids 'I, L, W, C' as the most important for distinguishing drought-responsive proteins.  
- Feature importance chart provides a visual understanding of amino acids contributing most to stress response.
# Requirements
Python, Biopython, NumPy, Pandas, Scikit-learn, Matplotlib.
