# Convex Optimization and Math for Linear Models
**Author:** B Chandu Chowdary, M.Tech (NIT)
---

## Folder Structure
Final/
├── Exe_Notebooks/  
│   ├── Equations/  
│   ├── preprocessed_df.pkl  
│   ├── Question_1.ipynb  
│   ├── Question_2.ipynb  
│   ├── Question_2F.ipynb  
│   └── Question_3.ipynb  
├── HTML_Scripts/  
└── PDFS/  

---

# California Housing (Linear Regression)

## Summary
- Target: MedHouseVal  
- Methods: Linear Regression + Ridge  
- Features: Polynomial + interaction terms  
- Training: Batch GD and Mini-Batch GD  

## Top Features
- Medinc_log²  
- spatial_proximity_score²  
- Medinc_log × AveRooms  
- Medinc_log × Population  
- AveRooms × spatial_proximity_score  

## Performance
- Best R² ≈ 0.68  
- Mini-Batch (10%) performs best  
- Simplified 3-feature model also reaches R² ≈ 0.68  

---

# Polynomial + LASSO Regression

## Results
- MSE: 5.6105  
- R²: –3.2135  

## Interpretation
- Polynomial expansion did not help  
- LASSO removed most features → underfitting  
- Worse than mean prediction  

---

# Breast Cancer – Logistic Regression

## Model
- Logistic Regression with L2 penalty  
- Solvers: GD, SGD, Mini-Batch (32, 64), SAGA  

## 5-Fold CV Accuracy
- GD: 0.9469  
- SGD: 0.9646  
- Mini-Batch 32/64: 0.9558  
- SAGA: 0.9558  

## Train vs Test Loss
- Very small gap → minimal overfitting  

## Lambda (λ) Effect
- Smaller λ → slightly higher accuracy  
- Larger λ → more regularization  

---

