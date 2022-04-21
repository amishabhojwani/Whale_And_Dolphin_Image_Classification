# Code for Cetacean Image Classification

The code for this project can be split in two batches:

- Exploratory and experimental analysis
    - `Species_and_Family_Image_Arrays.ipynb`
    - `First_Models_Family.ipynb`
    - `First_Models_Species.ipynb`
- Final modelling
    - `Resize_Images_and_Subset_to_Directories.ipynb`
    - `Image_Generator_Deep_Learning.ipynb`

The exploratory and experimental batch of code starts with `Species_and_Family_Image_Arrays.ipynb` which outputs pickles of two sampled datasets, one with balanced classes for families and one for species. These pickles are read into `First_Models_Family.ipynb` and `First_Models_Species.ipynb` to build tentative Convolutional Neural Networks which predict classifications of images to either Species or Family level with varying success.

The final modelling uses an image data generator approach to modelling in order to palliate RAM overconsumption. It starts with `Resize_Images_and_Subset_to_Directories.ipynb` which downsizes image dimensions and reorganises them into training and testing directories. These directories are called from `Image_Generator_Deep_Learning.ipynb` by image generators to feed Convolutional Neural Networks in batches of images.

#### Disclaimers
- The data used is not available on this repository as it is from the [Happy Whale Dolphin and Whale Identification Kaggle Competition in 2022](https://www.kaggle.com/c/happy-whale-and-dolphin?msclkid=378742b3c18711ec84d2d084acce762e).
- The directories correspond to those in a Kaggle working environment
- Python dependencies are listed at the beginning of each notebook but can also be found in dependencies.txt. The version of Python used is: `Python 3.9.7`.