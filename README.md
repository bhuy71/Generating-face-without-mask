# Unmask System. Reconsstructing Faces Beyond the Mask — Group 16


## Introduction
![Logo](https://github.com/user-attachments/assets/9f9680e0-e058-4fa0-983c-972cb8ba9451)


## Face Mask Detection Project

In an era where public health and safety are paramount, understanding and detecting the presence of face masks has become a crucial task.

This project represents our team’s initiative to develop a model capable of detecting face masks in images. Leveraging the **Face Mask Lite** dataset, we designed a machine learning pipeline focused on efficiency and accuracy. Our system utilizes **Python** as the primary programming language, integrating popular libraries like Keras and Pytorch to build and train our detection model.

The application is lightweight, scalable, and optimized for practical use cases such as public monitoring systems and workplace compliance checks. It prioritizes accuracy while ensuring computational efficiency, making it adaptable for deployment in real-world scenarios.

***This project is intended for `educational purposes only`. The model's performance is subject to dataset limitations and does not guarantee flawless detection. It should not be used as a replacement for professional safety measures or health compliance systems.***


## Key features

- Data preprocessing and **exploratory data analysis** performed in Jupyter Notebooks with support from [Pandas](https://pandas.pydata.org/) and [Matplotlib](https://matplotlib.org/).
- **GAN-based model** implemented for mask removal and face image generation using [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/).
- **Face mask detection** integrated with [UNet](https://arxiv.org/abs/1505.04597) architecture for accurate segmentation and mask identification.
- **Diffusion model** integrated for inpainting and refining generated images, utilizing pre-trained weights from [Hugging Face Diffusers](https://huggingface.co/docs/diffusers/).
- Lightweight **GUI** built with Python using [Tkinter](https://docs.python.org/3/library/tkinter.html) for an interactive user experience.
- Deployment-ready script for model inference, optimized with [Flask](https://flask.palletsprojects.com/en/3.0.x/) to serve predictions via HTTP API.


## Project structure
- **BasicTFGan**: Contains the implementation of the GAN model using TensorFlow.  
- **Model using mask detection and Unet**: Implements face mask detection using UNet and combines GAN techniques.  
- **PretrainedDiffusion_2_Inpainting**: Directory for diffusion models used for inpainting masked areas.  
- **Exploratory Data Analysis.ipynb**: Notebook for analyzing and preprocessing the dataset.  
- **UnMaskUI.py**: Python script to run a lightweight UI for interactive mask removal.  
- **infer.py**: Script for running model inference on input images.  
- **install.sh**: Shell script for setting up required dependencies.  
- **README.md**: Documentation explaining the project, features, and usage instructions.


## Requirements
Referring to our libraries used: `pip install -q -r requirements.txt`


## Installation and usage

Alongside


## GUI

Please refer to these following links for essential document:

+You can download data from this link:https://www.kaggle.com/datasets/prasoonkottarathil/face-mask-lite-dataset

+Data for training mask detection model:https://drive.google.com/drive/folders/1YSau5CWdgtpQGOpCvqhKLqvBwnVrO7jw?usp=sharing

+Premium GAN (pytorch model) checkpoints can be download here:https://drive.google.com/drive/folders/1JktC1krdN7wD1XqfuDTwnlsClhQaZ1Kg?usp=drive_link

Apart from creating the infer.py script following the teaching assistant's instructions, we have implemented an additional user-friendly interface. This interface allows users to run our code more conveniently through an intuitive GUI.

### infer.py


+Diffusion checkpoint can be downloaded here: https://drive.google.com/file/d/186KQQTm-MmXlFYh1MzB2NUWw5KZsRqWk/view?usp=sharing

+BasicTFGan checkpoint (Keras model) can be downloaded here: https://drive.google.com/file/d/1vjCB1Q21YFjnUDGkui1DrJsFLC7ztLlc/view?usp=sharing

+How to run this application . In UnMaskUI.ipynb :
  1. Paste the model path to the param:
     + KERAS_MODEL_PATH=<path_to_keras_model>
     + PYTORCH_MODEL_PATH=<path_to_pytorch_model>
     + DETECTION_MODEL_PATH=<path_to_detection_model>
     + DIFFUSION_MODEL_PATH=<path_to_diffusion_model>
  2. Run all the cell 
  3. After execute the last cell , there will be a link. You can experience by yourself now

### GUI
+Or you can run another way: ipython UnMaskUI.py . It will show a link too, click on that link to experience our application

+How to run Premium GAN:

  1.After clone this repository to local, you need to download checkpoint from the link above.

  2.You open file test_gan.ipynb and change the path to the checkpoint, mask detection YOLO model as well as the path to your image
  you want to generate.Then you run the final cell , the image generated will be saved in a folder, it also display on the screen for you.
  Note: Because of source of data , it can not work very well in real world.
  
*** How to run infer.py:

    First run install.sh

   1. To run with the PyTorch generator model:

     python script.py --model PyTorch Generator --pytorch_model_path /path/to/pytorch/model --input /path/to/input/image --output output.png

   2. To run with the Diffusion generator model:

     python script.py --model Diffusion Generator --diffusion_model_path /path/to/diffusion/model --input /path/to/input/image --output output.png

   3. To run with the Keras generator model:

     python script.py --model Keras Generator --keras_model_path /path/to/keras/model --input /path/to/input/image --output output.png


## Demo
![Demo](https://github.com/user-attachments/assets/51e5dfe0-7586-47ba-92c2-5a233c3fca9f)


## Acknowledgments
This project would not have been possible without the invaluable contributions of several open-source libraries, such as [Keras](link Keras), [PyTorch](link Pytorch), and [Diffusers](link Diffusers). Their robust tools and resources were instrumental in the success of this project.

We extend our heartfelt gratitude to our lecturers, Professor Nguyen Hung Son and Professor Trang Viet Chung, for assigning us this challenging yet captivating project. It has been an incredible learning opportunity that has significantly enhanced our knowledge and skillset.

Our sincere thanks also go to our teaching assistants, Doan The Vinh and Nguyen Ba Thiem, for their unwavering support and constructive feedback throughout the project. 

Finally, we would like to acknowledge our peers for their indirect contributions, offering both moral and practical support that kept us motivated and


## Contributors
- Lại Trí Dũng - 20225486
- Đỗ Đình Hoàng - 20225445
- Bùi Văn Huy - 20225497
- Vũ Việt Long - 20225508
- Trịnh Huynh Sơn - 20225526


## License
This project is licensed under the [MIT License](LICENSE).
