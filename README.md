
# Face vs. Non-Face Classification

This project implements a **Face vs. Non-Face Classification system** using **Principal Component Analysis (PCA)**, **Linear Discriminant Analysis (LDA)**, and **K-Nearest Neighbors (KNN)**. The goal is to classify whether an image contains a human face or not.

---

## 📂 Project Structure
- `facerec.ipynb` → Main Jupyter Notebook with all experiments and results  
- `archive3.zip` → Contains dataset files (faces and dummy non-faces)  

---

## ⚙️ Methodology
1. **Dataset Preparation**
   - Face images: Extracted from a standard face dataset.
   - Non-face images: 300 dummy non-face images generated.
   - Training and testing splits used (e.g., 330 train / 150 test).

2. **Dimensionality Reduction**
   - **PCA** applied to extract principal features from images.
   - **LDA** applied after PCA for maximizing class separability.

3. **Classification**
   - **KNN classifier** trained on reduced feature space.
   - Tested with different configurations of non-face images.

---

## 📊 Results
### Face vs. Non-Face (Example: 50 Non-Face Images)
- Accuracy: **1.0000**
- Precision: **1.0000**
- Recall: **1.0000**
- F1-Score: **1.0000**
- ✅ No failure cases.

### PCA-Only Classification (Different Alpha Values)
| Alpha | # Components | Accuracy |
|-------|--------------|----------|
| 0.80  | 36           | 95%      |
| 0.85  | 51           | 95%      |
| 0.90  | 76           | 94%      |
| 0.95  | 115          | 94%      |

### PCA + LDA Pipeline
- PCA reduced dimensions: 115  
- LDA accuracy (39 components): **93.5%**  
- PCA-only accuracy: **94%**

---

## 🖼️ Example Predictions
- Successfully predicted both face and non-face images with high confidence.  
- All test cases shown in the notebook were classified correctly.  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/HANA5299/Face-no-Face-CLassification.git
   cd Face-no-Face-CLassification
   ```
2. Open Jupyter Notebook:
   ```bash
   jupyter notebook facerec.ipynb
   ```
3. Run all cells to reproduce results.

---

## 📌 Key Takeaways
- PCA is effective for feature extraction from facial images.
- Combining PCA + LDA improves class separability.
- KNN performed well with both PCA-only and PCA+LDA pipelines.
- Achieved **up to 100% accuracy** in face vs. non-face classification tasks.

---

## 📧 Contact
Developed by **Hana Ibrahim Elsayed Ibrahim**  
Feel free to connect for collaborations or improvements!  
