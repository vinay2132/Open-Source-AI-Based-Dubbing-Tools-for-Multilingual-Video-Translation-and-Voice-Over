

# Deep Learning Approach for Gender and Age Prediction Using CNN

## Overview  
This project develops a Convolutional Neural Network (CNN) model to accurately predict gender and age from facial images. The model leverages deep learning techniques and a multi-output architecture to simultaneously estimate these attributes. Applications include advertising, healthcare, and security, where demographic analysis and personalization are key.

## Features  
- **Multi-Output CNN Architecture**: Predicts both age and gender in a single pass.  
- **High Accuracy**: Achieves 90% accuracy for gender classification and a Mean Absolute Error (MAE) of 6.5 for age prediction.  
- **Robust Preprocessing**: Uniform image resizing and grayscale conversion for optimal feature extraction.  
- **Real-World Applications**: Enhances decision-making in industries such as marketing, security, and healthcare.  

## Dataset  
The project uses the [UTKFace dataset](https://www.kaggle.com/jangedoo/utkface-new) comprising 23,708 labeled images. Images are resized to 128x128 pixels, with labels extracted directly from filenames for simplicity.  

## Model Architecture  
- **Input Layer**: Accepts preprocessed grayscale images.  
- **Convolutional Layers**: Extract hierarchical facial features.  
- **Max-Pooling Layers**: Downsample feature maps.  
- **Fully Connected Layers**: Learn relationships between features and target variables.  
- **Output Layer**: Provides predictions for gender and age.  

Dropout regularization is applied to prevent overfitting, and the Adam optimizer ensures efficient training.

## Results  
- **Gender Classification**: Achieved 90% accuracy.  
- **Age Prediction**: MAE of 6.5 with a standard deviation of 4.  

Graphs for training and validation loss, accuracy, and MAE demonstrate effective learning and generalization.  

## Installation and Usage  
1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/vinay2132/deep-learning-gender-age-cnn.git
   cd deep-learning-gender-age-cnn
   ```  
2. **Install Dependencies**:  
   Use `pip` to install required libraries:  
   ```bash
   pip install -r requirements.txt
   ```  
3. **Run the Model**:  
   Execute the script to train or evaluate the model:  
   ```bash
   python train_model.py
   ```  

## Challenges and Future Work  
- **Dataset Bias**: Address underrepresentation of certain age groups and gender identities.  
- **Environmental Variations**: Improve resilience to changes in lighting, orientation, and expression through data augmentation.  
- **Generalization**: Enhance performance across diverse datasets for broader applicability.

## Acknowledgments  
We thank the authors of related works for their insights and the UTKFace dataset providers. Gratitude also extends to our mentors, colleagues, and supporters who made this research possible.

## Authors  
- **Vinay Daram** ([LinkedIn](https://www.linkedin.com/in/daramvinay)) 

## License  
This project is licensed under the MIT License. See the `LICENSE` file for details.
