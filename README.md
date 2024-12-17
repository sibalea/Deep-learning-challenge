# Deep-learning-challenge
Script file: `AlphabetSoupCharity.ipynb`
optimization file: `AlphabetSoupCharity_Optimization.ipynb`
Models: `models/first_model.h5`
`checkpoints`
<>
Step 1: Preprocess the Data
Step 2: Compile, Train, and Evaluate the Model
Step 3: Optimize the Model
To optimize our model, we deepen thhe learning by changing varius data in the data set. 
First, we created more hidden layers up to 4,
2nd, we tried numerous epochs from 100 to 700 then back to 50.
3rd, we adjust the time from 0.1 to 0.01, then 0.0001 to allow more learning time.
4th, we use Adam, then Nadam, even tried embbeding.
None of this optimization could get us above 74% accuracy. Actullay, with the increase hidden layers and dense change, we notice a decrease in accuracy.
Step 4: Write a Report on the Neural Network Model

The report is a summary of the performance of the deep learning model we created for Alphabet Soup.


    Overview of the analysis: 
    Purpose of the analysis
Create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

    Results: Using bulleted lists and images to support your answers, address the following questions:

    Data Preprocessing
        What variable(s) are the target(s) for your model?
        What variable(s) are the features for your model?
        What variable(s) should be removed from the input data because they are neither targets nor features?

    Compiling, Training, and Evaluating the Model
        
Compiling, Training, and Evaluating the Model

    Model Architecture:
    The neural network consists of:

        Input Layer: This is implicitly defined by the input_dim=43, meaning the model receives 43 features as input.

        First Hidden Layer: 80 neurons with ReLU activation.

        Second Hidden Layer: 30 neurons with ReLU activation.

        Output Layer: 1 neuron with sigmoid activation for binary classification.

        Total Layers: 3 layers (2 hidden layers and 1 output layer).

        Neurons: 80 neurons in the first hidden layer, 30 neurons in the second hidden layer, and 1 neuron in the output layer.

        Activation Functions:
            ReLU (Rectified Linear Unit) is used for the hidden layers.
            Sigmoid is used for the output layer to output values between 0 and 1, indicated for binary classification.

    Achieving Target Model Performance (75%):
    Whether this model can achieve the 75% performance target depends on multiple factors such as:
        Data Quality: If the data is clean, balanced, and properly preprocessed, the model can potentially reach or exceed 75%.
        Training Process: Proper optimization and tuning (e.g., using the Adam optimizer, learning rate adjustments, and dropout for regularization) will affect model performance.
        Hyperparameters: Tuning the number of neurons or layers, changing activation functions, or using different batch sizes may improve the results.

    Steps to Improve Performance:
        Hyperparameter Tuning: Experiment with different numbers of neurons, activation functions, and layers.
        Regularization: Add dropout layers to avoid overfitting.
        Data Augmentation or Synthetic Data: If the dataset is small or imbalanced, consider techniques like oversampling the minority class or generating synthetic data.
        Learning Rate Adjustment: Use learning rate schedules or adaptive learning rates like Adam optimizer.
        Cross-validation: Implement k-fold cross-validation to ensure the model generalizes well.

    Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Step 5: Copy Files Into Your Repository

Now that you're finished with your analysis in Google Colab, you need to get your files into your repository for final submission.