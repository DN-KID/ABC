#  Adaptive Blank Compensation for Few Shot Image Classification


## Backbone Training

We use the same backbone network and training strategies as 'S2M2_R'. Please refer to https://github.com/nupurkmr9/S2M2_fewshot for the backbone training.

## Extract and save features

After training the backbone as 'S2M2_R', extract features as below:

- Create an empty 'checkpoints' directory.

- Run:
```save_features
python save_features.py --dataset [miniImagenet/CUB/CIFAR-FS] 
```
### Or you can directly download the extracted features/pretrained models from the link:
https://drive.google.com/drive/folders/1plWYjXC-9-to1v2sXq94NCPq_mE0dChJ?usp=sharing


After downloading the extracted features, please adjust your file path according to the code.


## Evaluation

To evaluate our ABC method, run:

```eval
python CABC.py
```
