-

# SNN Classification and Colorization Results  

## 1. Spiking Neural Network (SNN) + CNN for Animal Detection  

**Performance Metrics:**  
- **Testing Accuracy:** 84.46%  
- **Precision, Recall, F1 Scores:** High across weighted, macro, and micro averages.  

| Metric               | Value    |
|-----------------------|----------|
| Weighted Precision    | 0.8460   |
| Weighted Recall       | 0.8446   |
| Weighted F1 Score     | 0.8447   |

**Class-Specific Performance:**  
- Balanced performance across most classes, except for slightly lower precision in Class 1.  

![SNN Predictions](https://github.com/user-attachments/assets/e17b2ec3-17b1-4bad-b902-45809291b936)  

---

## 2. ANN-CNN Hybrid for Animal Detetection 

**Performance Metrics:**  
- **Testing Accuracy:** 66.56%  
- **Mean Squared Error (MSE):** 0.0085  
- **PSNR:** 70.9543 dB  
- **SSIM:** 0.7645  

| Metric               | ANN-CNN  | SNN       |
|-----------------------|----------|-----------|
| Test Loss (MSE)      | 0.0085   | 0.0127    |
| PSNR (dB)            | 70.95    | 19.51     |
| SSIM                 | 0.7645   | 0.8024    |

**Visual Comparison:**  
![Comparison 1](https://github.com/user-attachments/assets/a53d4a54-9118-49f2-adcc-f70c6ab230f1)  
 

---

## Comparative Analysis  

**Key Observations:**  
1. **SNN vs. ANN-CNN for Detection:**  
   - SNN outperformed ANN-CNN by **17.9% in accuracy**.  
   - SNN demonstrated better generalization with balanced class performance.  

2. **SNN-CNN vs. ANN-CNN for Colorization:**  
   - ANN-CNN produced higher-quality outputs with a lower MSE and higher PSNR.  
   - SNN achieved better structural similarity (SSIM), but results were noisier.  

**Histogram**

SNN-CNN :

![colorization](https://github.com/user-attachments/assets/507260c6-c9f3-4c92-9b53-532fd2964183)

![Histogram Comparison](https://github.com/user-attachments/assets/0695c999-77a8-460f-938c-c4c031016958)  

ANN-CNN :

![WhatsApp Image 2024-11-22 at 21 07 08_d05a2975](https://github.com/user-attachments/assets/47867d34-a593-4414-8af2-4d3d61eb0514)

![Comparison 2](https://github.com/user-attachments/assets/90a97b82-7b70-4457-adf9-f93b72983b7c) 

---

## Limitations and Future Work  

- **SNN:** Needs optimization to reduce noise and improve smoothness in pixel predictions.  
- **ANN-CNN:** Computationally intensive but superior for high-accuracy tasks.  
- **Next Steps:** Explore transfer learning, surrogate gradient methods, and edge-case augmentations for SNN.  


