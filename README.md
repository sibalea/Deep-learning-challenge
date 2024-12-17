# Deep-learning-challenge
Overview of the analysis: 
    Purpose of the analysis
Create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
Data files
Script file: `AlphabetSoupCharity.ipynb`
optimization file: `AlphabetSoupCharity_Optimization.ipynb`
Models: `models/first_model.h5`
`checkpoints`
<>
Step 1: Preprocess the Data
Step 2: Compile, Train, and Evaluate the Model
Step 3: Optimize the Model
To optimize our model, we deepen thhe learning by acting simultoneously on many factors in the set. 

First, we created more hidden layers up to 4. We also decrease features from 43 to 40, via 42.

2nd, we tried numerous epochs from 100 to 700 then back to 50.

3rd, we adjust the learning rate from 0.1 to 0.01, then 0.0001 to allow more learning time.

4th, we use Adam optimizer, then Nadam. We even tried embbeding.

None of these optimization changes increased the accuracy above 74% . Actullay, with the increase hidden layers and units change, we notice a decrease in accuracy.


    Steps to Improve Performance:
        Hyperparameter Tuning: Experiment with different numbers of neurons, activation functions, and layers.
        Regularization: Add dropout layers to avoid overfitting.
        Data Augmentation or Synthetic Data: If the dataset is small or imbalanced, consider techniques like oversampling the minority class or generating synthetic data.
        Learning Rate Adjustment: Use learning rate schedules or adaptive learning rates like Adam optimizer.
        Cross-validation: Implement k-fold cross-validation to ensure the model generalizes well.


Step 5: Copy Files Into Your Repository