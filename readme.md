# Pokemon Incubator

## Introduction
This is a Pokemon incubator for generating new monsters using GAN and improved WGAN. Please look at the poster_latext_2.pdf for further introduction and contributors.

## Train

1. Save training images to folder `training-data`

2. Run training script

```bash
python train.py --epochs=100 --batch-size=32 \
    --sample-interval=50 --load-saved=True --method=wgangp
```

## Example Results

![epoch_850](examples/epoch_850.png)
![epoch_1300](examples/epoch_1300.png)
![epoch_6600](examples/epoch_6600.png)
![epoch_7450](examples/epoch_7450.png)
![epoch_17400](examples/epoch_17400.png)


<details>
<summary>Why not fork?</summary>
It's a great repo to fork and start with, but there are too many GAN implementations that we are not going
to use. So we copied the code we need and modified them for our training sets.
</details><br/><br/>

[utils](utils.py) is taken and modified from 
[Pokemon_GAN](https://github.com/llSourcell/Pokemon_GAN/blob/master/utils.py).

<details>
<summary>Why not fork?</summary>
Again, a great repo that taught us a lot, but we wanted to try different algorithms to train our data.
</details>
