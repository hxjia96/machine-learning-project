# machine-learning-project
Using fizyr's implementation Keras RetinaNet to train a object detection model on rose and sunflower
## model
### Retinanet
backbone:resnet50
class: rose
       sunflower
train set: 600 images
batch size: 1
step:600
epoch:30

## Train
Using retinanet/train.py
example:

`keras_retinanet/bin/train.py csv /path/to/csv/file/containing/annotations /path/to/csv/file/containing/classes`

## Converting a training model to inference model
Using retinanet/convert_model.py
example:

`keras_retinanet/bin/convert_model.py /path/to/training/model.h5 /path/to/save/inference/model.h5`

## Test
Using retinanet/test.ipynb
result example:
<img src="https://github.com/hxjia/machine-learning-project/master/result1.png" />
<img src="https://github.com/hxjia/machine-learning-project/master/result2.png" />
