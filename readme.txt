Cross Modal Semantic Learning for Image Captioning

This project is a python based application that generates captions for images. It bridges the connection between Computer Vision and Natural Langauge Processing.

Overview
This project focuses on automatically generating captions for images using deep learning. The model learns to associate visual content with textual descriptions, making it useful for applications like image-based search, accessibility for visually impaired users, and AI-driven content generation.

Features
-Automated Image Captioning: Generates textual descriptions for images without human  intervention.
-Cross-Modal Learning: Connects visual data with natural language descriptions.
-LSTM Decoder: Generates image captions by processing extracted image features  sequentially.
-VGG16 Encoder: Extracts meaningful features from images using a pre-trained  convolutional neural network.
-Scalability: Can be expanded to work with larger datasets like MS COCO.
-Real-World Applications: Useful for assistive technologies, content tagging, and   multimedia retrieval.

Project Structure
├── .ipynb_checkpoints #will be created when file is run in Jupyter 
├── Input  
     ├── Images                   
     ├── Captions                                 
├── Features.pkl  #will be created after extraction of features           
├── Project_code            
├── requirements.txt    
├──readme.txt


Requirements
- Python
- Google Colab or Jupyter Notebook
- modules
 - tensorflow
 - numpy
 - matplotlib
 - pillow
 - tqdm
 - nltk
 - pickle  

Dataset
Flickr8k dataset 
dataset kaggle link: https://www.kaggle.com/datasets/hsankesara/flickr-image-dataset

Dataset Setup
1. Download the dataset manually from the above link or use the Kaggle API to download it directly.
2. Once downloaded, extract the dataset so that the Flickr_8k_Dataset folder (containing images) and Flickr8k.token.txt (captions file) are in the root directory of the    project.
3. The folder structure should look like this:
   project_root
      ├──Dataset
	├── Flickr_8k_Dataset/  # Folder containing images
	├── Flickr8k.token.txt  # Captions file
      ├── your_script.py

Setup
Make sure to install required dependencies which are present in the requirements.txt via python command 'pip'.

Usage
1. Verify Dataset and Dependencies
 - Ensure that the Flickr 8k Dataset is correctly placed in the root directory as mentioned in the dataset setup.
 - Install the necessary dependencies using:
	pip install -r requirements.txt

2. Run the Notebook
  -Open the Notebook in the google colab or Jupyter Notebook and run the notebook cell by cell

3. Generate Captions
  -After running all the notebook cells, use the generate_caption() function to get captions for an image:
        caption = generate_caption("Flickr_8k_Dataset/example.jpg")
	print(caption)
  -The model will generate a caption for the given image based on trained data.

References
 -https://www.youtube.com/watch?v=fUSTbGrL1tc&pp=ygUmaW1hZ2UgY2FwdGlvbiBnZW5lcmF0b3IgcHl0aG9uIHByb2plY3Q%3D
 -https://www.geeksforgeeks.org/vgg-16-cnn-model
 -https://www.sciencedirect.com/science/article/abs/pii/S0167278919305974
 -https://www.sciencedirect.com/science/article/pii/S0925231223004101











             


