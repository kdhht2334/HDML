# Hardness-Aware Deep Metric Learning
Implementation of Hardness-Aware Deep Metric Learning in Tensorflow.

- HDML:  [Hardness-Aware Deep Metric Learning](http://.pdf)


# Dependencies
```bash
pip install tensorflow==?
```

# Dataset
Stanford Cars Dataset (Cars196)

可从官网 (https://ai.stanford.edu/~jkrause/cars/car_dataset.html) 或者使用lib/datasets/cars196_downloader.py文件下载，并使用cars196_converter.py转化为h5py文件，放在lib/datasets/data/cars196

# Usage
## For Cars196 dataset:

```bash
python CVPR_main_HDML_npair.py --dataSet='cars196' --batch_size=128 --Regular_factor=5e-3 --init_learning_rate=7e-5 --load_formalVal=False --embedding_size=128 --loss_l2_reg=3e-3 --init_batch_per_epoch=500 --batch_per_epoch=64 --max_steps=8000 --beta=1e+4 --lr_gen=1e-2 --num_class=99 --_lambda=0.5 --s_lr=1e-3
```

lr decay at 5632 6848.


# Code Reference
deep\_metric\_learning (https://github.com/ronekko/deep_metric_learning) by [ronekko](https://github.com/ronekko)
