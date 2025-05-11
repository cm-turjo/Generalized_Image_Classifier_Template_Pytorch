
# Generalized Pytorch Image Classifier Template

This is a generalized pytorch image classifier template where one can find models from timm library. The is designed in such a way that it adapts automatically to the required image size of the given model and applies various transformation of the training images through RandAugment function available in timm library and pytorch. The code after training, produces information about

- Print log information such  as training loss,  validation loss, training accuracy and validation accuracy per epoch with smooth progress bar for training and validation
- Save these information into an excel file on the output directory
- After training completes the code prints loss vs epoch curve and accuracy vs epoch curve and saves them as figures.
- The code also save model checkpoint information of every epoch along with optimizer state so that you can download and retrain later
- After choosing which epoch's checkpoint to be loaded, you can test the model performance by observing classification report and confusion matrix and saved them
- There is a dedicated model finder section, using regex you can find and check which model to load and experiment on.
- Seed feature to maintain reproducibility feature




## Dataset Structure
The dataset should be divided in:

- Train
- Validation
- Test

Modify the name according to your dataset in the CFG section or configuration section.
## Hyper Parameter Section

You can change batch size, number of epcohs, learning rate, seed and other information
## How to Run it
For Kaggle
- Open Kaggle Account
- Verify your phone number to access GPU
- Divide the dataset according to the given structure
- Select Tesla P100 (Recommended) as the GPU Accelarator
- Run the Notebook

For Local PC
- Configure CUDA cores 
- Install Anaconda for Jupyter Notebook (Recommended)
- Run the Notebook