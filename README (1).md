Food Image Recognition Using CNN Inception V3


## Dependencies

- TensorFlow
- Keras
- Matplotlib
- Numpy
- Scikit-learn
- CV2
- Pandas
- OS
- PIL

You can install all Dependencies using the following command: 
```python
pip install -r requirements.txt
```

Ensure you have a requirements.txt file in your repository listing all the dependencies.
## Authors

- [@xyzaraa](https://github.com/xyzaraa)
- [@alviyalaela](https://github.com/alviyalaela)
- [@Zahwabmz1562](https://github.com/Zahwabmz1562)



## Source Dataset
Our dataset is combined from these 3 source:

Food Image Dataset: 
[Kaggle](https://www.kaggle.com/code/artgor/food-recognition-challenge-eda)

Indonesian Food Image:
[data-mendeley](https://data.mendeley.com/datasets/vtjd68bmwt)

Indonesian Food Image (2):
[roboflow](https://universe.roboflow.com/traditional-food/traditional-foodv1)
# Usage
Recommended to use google colab

## Setup Dataset
Download the 
[dataset](https://drive.google.com/drive/folders/1LWnoDDsqY1ixVTtD1Pl0w39D-Hwvssdo?usp=sharing) first and upload to your Google Drive. Use this code to mount google drive in colab
```python
from google.colab import drive
drive.mount('/content/drive')
```

## Load the Model and CSV

Download model above (Inception V3) and CSV for the nutrition

```python
be.clear_session()
model_path = "./model_inceptionV3.h5"
print("loading the model..")
model = load_model(model_path)
```
    
## Running Tests

To run tests, run the following command

```python
predict_image(<file_path>, model)
```

