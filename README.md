# Generating-face-without-mask
+You can download data from this link:https://www.kaggle.com/datasets/prasoonkottarathil/face-mask-lite-dataset

+Pytorch and Mask Dectecion checkpoints can be download here:https://drive.google.com/drive/folders/1JktC1krdN7wD1XqfuDTwnlsClhQaZ1Kg?usp=drive_link

+Data for training mask detection model:https://drive.google.com/drive/folders/1YSau5CWdgtpQGOpCvqhKLqvBwnVrO7jw?usp=sharing

+Keras checkpoint can be download here: 

+Diffusion checkpoint can be downloaded here: https://drive.google.com/file/d/186KQQTm-MmXlFYh1MzB2NUWw5KZsRqWk/view?usp=sharing

+How to run this application . In UnMaskUI.ipynb :
  1. Paste the model path to the param:
     + KERAS_MODEL_PATH=<path_to_keras_model>
     + PYTORCH_MODEL_PATH=<path_to_pytorch_model>
     + DETECTION_MODEL_PATH=<path_to_detection_model>
     + DIFFUSION_MODEL_PATH=<path_to_diffusion_model>
  2. Run all the cell 
  3. After execute the last cell , there will be a link. You can experience by yourself now

+Or you can run another way: ipython UnMaskUI.py . It will show a link too, click on that link to experience our application
