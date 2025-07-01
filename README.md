# KNN-CLASSIFICATION
TASK 6:KNNCLASSIFICATION
# 🛳️ Titanic K-NN Classification with Decision Boundaries

This project uses *K-Nearest Neighbors (K-NN)* on the Titanic dataset to:
- Normalize features
- Try different values of K
- Evaluate performance (accuracy, confusion matrix)
- Visualize decision boundaries

---

## 📂 Dataset

We use the built-in Titanic dataset from seaborn:

python
df = sns.load_dataset('titanic')


Selected columns:
- Features: pclass, sex, age, sibsp, parch, fare, embarked
- Target: survived

---

## ⚙️ Tasks Performed

### 1. Data Preprocessing
- Dropped rows with missing values
- One-hot encoded categorical variables
- Split into training and testing sets (80/20)

### 2. Normalization
- Used StandardScaler to normalize feature values for better K-NN performance

### 3. K-NN Classifier
- Applied KNeighborsClassifier from sklearn.neighbors
- Experimented with k values: 3, 5, 7, 9, 11
- Selected the best k using accuracy

### 4. Evaluation
- Accuracy score for each k
- Confusion matrix for best model (ConfusionMatrixDisplay)

### 5. Decision Boundary Visualization
- Used only 2 features: age and fare
- Plotted decision surface using meshgrid and contour plot

---

## 📈 Output

- Accuracy for different k values printed in console
- Confusion matrix displayed for best model
- 2D decision boundary plot using age and fare

---

## 🧰 Libraries Used

text
pandas
numpy
seaborn
matplotlib
scikit-learn


---

## ▶️ How to Run

1. Install the required libraries (if not installed):

bash
pip install pandas numpy matplotlib seaborn scikit-learn


2. Copy and paste the full Python code into a Jupyter Notebook or Python script.
3. Run the code. You will see:
   - Accuracy results
   - Confusion matrix
   - Decision boundary plot

---

## 📝 Example Output

text
k=3  | accuracy=0.765
k=5  | accuracy=0.780
k=7  | accuracy=0.773
k=9  | accuracy=0.765
k=11 | accuracy=0.758


- Best k: 5
- Accuracy: 78%
- Confusion matrix and decision boundary will be shown

---

## 📌 Notes

- This is for educational purposes.
- Titanic is a small dataset; K-NN may not give the best real-world performance.
- This project helps understand:
  - How K-NN works
  - The effect of different values of k
  - Visualizing classification boundaries in 2D

---

## ✍️ Author

*Sharmila L*  
