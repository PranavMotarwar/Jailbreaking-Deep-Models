# Jailbreaking Deep Models: Adversarial Attacks  
![License](https://img.shields.io/badge/License-MIT-blue)

**Authors**: Aniket Mane, Subhan Akhtar, Pranav Motarwar  
**Affiliation**: New York University  
**GitHub**: [Repository Link](https://github.com/PranavMotarwar/Jailbreaking-Deep-Models)  

---

## 📂 Repository Contents
| File/Folder       | Description                                  |
|--------------------|----------------------------------------------|
| `DL_project_3.ipynb` | Jupyter Notebook with full implementation    |
| `task5_transferability.png` | Graph for Task 5 results                  |
| `Deep_Learning_Mini_Project_3.pdf` | Project report (PDF)             |

---

## ▶️ Quick Start
1. **Run in Colab**:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HIQl6CYfBTWDs2_ccNa0NRFR0nYTTb2i?usp=sharing)

2. **Local Execution**:
   ```bash
   # Install dependencies
   pip install -r requirements.txt
   
   # Launch Jupyter notebook
   jupyter notebook DL_project_3.ipynb

📊 ResNet-34 Accuracy Across Attack Types

The graph below shows the Top-1 and Top-5 classification accuracy of the ResNet-34 model on clean and adversarially perturbed datasets using FGSM, PGD, and Patch-PGD attacks.

![ResNet Accuracy](Task4result.png)

	•	Clean data yields strong performance (Top-1: 76%, Top-5: 94%).
	•	FGSM reduces Top-1 to 6%, showing high vulnerability to fast gradient attacks.
	•	PGD (iterative FGSM) nearly breaks the model (Top-1: 0%, Top-5: 2%).
	•	Patch-PGD partially preserves model performance (Top-1: 39%, Top-5: 76%).

These results demonstrate the fragility of ResNet-34 under adversarial pressure, especially from iterative perturbations like PGD.

📊 Task 5: Transferability Graph

Transferability Results
*DenseNet-121 performance across adversarial datasets.
PGD attacks show strong cross-model transferability.*

![DenseNet-121 Performance on Adversarial Datasets](Results.png)

**Key Observations**:
- **Original**: 75.00% Top-1 accuracy — strong baseline performance. (baseline)  
- **FGSM**: Accuracy drops to 63.00%, showing a 12% absolute decrease.
- **PGD**: Top-1 accuracy further drops to 53.00%, indicating a 22% absolute degradation from clean performance.
- **Patch PGD**: Partial recovery with 71.00% Top-1 accuracy, showing that localized attacks are less effective and less transferable to DenseNet-121.

*Visualization shows adversarial examples crafted for ResNet-34 significantly degrade DenseNet-121 performance, demonstrating cross-model vulnerability.*

📄 Report Highlights

Key findings from Deep_Learning_Mini_Project_3.pdf:

Reduced ResNet-34 accuracy to 0.00% using PGD (ε=0.02)

Patch attacks (32x32, ε=0.3) achieved 41.20% Top-1 accuracy

FGSM perturbations transferred to DenseNet-121 with 63.40% Top-1 accuracy


🔍 How to Reproduce Results

Download TestDataSet.zip and unzip.

Run cells attached ipynb sequentially.

Results auto-generated in notebook and saved as PNG/PDF.



---

## 🤝 Acknowledgements

This project was completed as part of the **Deep Learning course at NYU Tandon School of Engineering** in **Spring 2025**.

We would like to thank our professor and teaching assistants for their support and guidance throughout the project.

---
