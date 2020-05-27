# Keras Drop-Connect

![](https://img.shields.io/badge/keras-tensorflow-blue.svg)
![](https://img.shields.io/badge/keras-tf.keras-blue.svg)
![](https://img.shields.io/badge/keras-tf.keras/eager-blue.svg)
![](https://img.shields.io/badge/keras-tf.keras/2.0.0_beta-blue.svg)


## Install

```bash
pip install git+https://github.com/jernsting/keras-drop-connect
```

## Usage

Set drop connect rate for all weights:

```python
import keras
from keras_drop_connect import DropConnect

DropConnect(
    layer=keras.layers.Dense(units=10),
    rate=0.2,
)
```

Set drop connect rate with a dict:

```python
import keras
from keras_drop_connect import DropConnect

DropConnect(
    layer=keras.layers.Dense(units=10),
    rate={'kernel': 0.2},
)
```
