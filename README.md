PRODIGY_ML_03

🎯 Task 03 - Image Classification using Support Vector Machine (SVM)

This task is part of my internship at Prodigy Infotech, where I implemented an SVM-based image classifier to distinguish between images of cats and dogs using the Kaggle dataset.

📌 Objective

Build a machine learning model using Support Vector Machine (SVM) to classify cat and dog images by training it on labeled data from the Kaggle Dogs vs. Cats dataset.

📊 Dataset Used

- Source: [Kaggle - Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats/data)
- File: `train.zip`
- Contains 25,000 labeled images named as `cat.x.jpg` or `dog.x.jpg`

⚙️ Technologies Used

- Python  
- Google Colab  
- Libraries:  
  - `OpenCV` (for image processing)  
  - `NumPy` (for array manipulation)  
  - `Matplotlib` (for visualization)  
  - `Scikit-learn` (for training SVM and evaluation)

🚀 How to Run the Project

1. Download the dataset from Kaggle and upload `train.zip` to Google Drive.
2. Mount Google Drive in Colab:

   from google.colab import drive
   drive.mount('/content/drive')

3. Unzip the Dataset using:

    import zipfile
zip_path = '/content/drive/MyDrive/YourFolder/train.zip'
extract_path = '/content/dogs-vs-cats'
with zipfile.ZipFile(zip_path, 'r') as zip_ref:
    zip_ref.extractall(extract_path)

4. Preprocess Images:

- Resize to 64×64
- Flatten to vectors
- Assign labels: 0 for cat, 1 for dog

5. Train the SVM Model:

- Use SVC(kernel='linear') from Scikit-learn
- Split data with train_test_split
- Evaluate with accuracy_score and classification_report

6. Visualize Results (optional):

- Display random prediction images and their predicted labels

  📂 Files Included
- task_03.ipynb – Jupyter Notebook containing full code
- README.md – This file (project documentation)


  📈 Sample Output (Accuracy Report)

  Accuracy: 0.85  # (Example result)
              precision    recall  f1-score   support

           0       0.86      0.84      0.85       100
           1       0.84      0.86      0.85       100

✍️ Author
Kashish Tomar
Intern at Prodigy Infotech – June 2025
GitHub: @kashishtomar-11
