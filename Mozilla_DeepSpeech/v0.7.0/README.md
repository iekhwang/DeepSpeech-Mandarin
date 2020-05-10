DeepSpeech v0.7.0
=====



Git the v0.7.0 version from DeepSpeech
-----


```
git clone https://github.com/mozilla/DeepSpeech.git
```
```
cd DeepSpeech
less VERSION
```

if the version is not v0.7.0, hard reset the version to v0.7.0

```
git reset --hard v0.7.0
```

Create a docker image and container on your server or laptop
-----

Create docker image
```
docker build -t mozilla_deepspeech:v0.7.0 .
```
Create docker container
```
nvidia-docker run -it -v $path/DeepSpeech:/DeepSpeech mozilla_deepspeech:v0.7.0 /bin/bash
```
Train your language model
-----

Please check the offical steps -> https://github.com/mozilla/DeepSpeech/tree/master/data/lm

Train your model
-----

Please check a tiny model for training -> https://github.com/mozilla/DeepSpeech/blob/master/bin/run-ldc93s1.sh

If you have problem with hyperparameters, you can check with ```python DeepSpeech.py --helpfull```

---------

If you have any problems with DeepSpeech v0.7.0, please do not hesitate to contact me with iekhwang@outlook.com
