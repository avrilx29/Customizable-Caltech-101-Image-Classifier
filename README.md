# Customizable-Caltech-101-Image-Classifier

An interactive command-line computer vision tool built by **Avril** that allows users to dynamically select categories and subsets from the Caltech-101 dataset to train a custom `fastai` image classification model.

## Features

* **Interactive Selection:** Prompts users to navigate through 5 main categories of the Caltech-101 dataset (Animals, Vehicles, Food & Plants, Objects & Electronics, Architecture & Culture) and pick specific subsets to classify.
* **Dynamic Data Filtering:** Automatically filters the local Caltech-101 image files based on user choices.
* **Automated Model Training:** Instantly sets up a `fastai` DataBlock and fine-tunes a `ResNet18` deep learning model using mixed-precision training.
* **Visual Test Predictions:** Automatically samples random test images from the chosen subsets, runs predictions, and plots the results with confidence scores using Matplotlib.

## Prerequisites & Dependencies

* **Python** (version 3.8 or higher recommended)
* **Python Libraries:**
  ```bash
  pip install fastai pandas matplotlib
* **Helpful Tip** This code trains a deep learning computer vision model (ResNet18). While it can run on a CPU, training will be significantly faster if you have a compatible NVIDIA GPU with CUDA installed. Alternatively, you can upload and run this script easily inside a notebook such as `Jupyter Notebooks` with a GPU runtime enabled!
*  **Note** The fastai library will automatically download and unpack the Caltech-101 dataset into your environment the first time you run the script:
untar_data(URLs.CALTECH_101)

## How to Run:

1. **Clone or Download** this repository to your local machine.
2. **Open your terminal or command prompt** and navigate to the folder where your `main.py` file is saved.
3. **Execute the script** by running:
   ```bash
   python main.py
4. **Follow the interactive prompts** in your terminal:
   * Enter your name when asked.
   * Specify how many main categories you want to explore (e.g., 2 or 3).
   * Type out the main category names (e.g., animals or vehicles) based on the options displayed.
   * Review the available subsets for your chosen categories.
   * Select how many subsets you want to classify and type them in.
   * Watch the script automatically filter the dataset, initialize the data block, and fine-tune the ResNet18 model!
5. **View Results:** Once training finishes, a Matplotlib window will pop up showing randomly sampled images from your chosen subsets along with the model's predictions and confidence scores.

## Acknowledgments & Credits

* **Creator:** Avril
* **Framework & Inspiration:** The core computer vision concepts and foundational code structure were adapted from the [fast.ai](https://www.fast.ai/) library and tutorials, then heavily modified and customized for this interactive Caltech-101 project.
* **AI Assistance:** Artificial intelligence tools were used to help debug, refactor, and streamline some sections of the Python code.
* **Dataset:** The Caltech-101 dataset was used to provide a wide range of high quality images for users to choose from.

