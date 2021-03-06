# face-verification
Facial Verfication model training based on Facenet

## Setup

Install Conda
https://www.anaconda.com/distribution/

Create a new environment and activate
```
conda create -n tf-keras python=3.7
conda activate tf-keras
```
Clone the repo
```
git clone https://github.com/mohankumarSriram/face-verification.git
```

Download facenet model [here](https://drive.google.com/open?id=1pwQ3H4aJ8a6yyJHZkTwtjcL4wYWQb7bn) and copy to the models folder

Download toy dataset [here](https://drive.google.com/open?id=1EfvaELfw9GrCKm9gythFTh8yUmfGSftV)
```
mkdir models
cp ~/Downloads/facenet_keras.h5 models/

unzip ~/Downloads/data.zip -d ./
```


Install requiremnts
```
pip install -r requirements.txt
```


## Load Dataset
```
python load_data.py
```

## Generate Embeddings
```
python generate_embeddings.py
```

## Train Classifier
```
python train_classifier.py
```

## Perform Inference
```
python infer.py
```