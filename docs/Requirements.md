# Image Classification using TensorBoard

## Installation

#### Requirements
* Python
* `Jupyter Notebook` or `Google Collab Notebook`
* `Numpy` version >=1.13.3
* `Pip` (*optional*)

#### Installing using pip

In pip is already installed or you have `Anaconda` distribution of python,

```
pip install tensorflow
```
```
pip install tensorboard
```
`tensorboard` comes along with `tensorflow` so we might see the following while installing `tensorflow` explicitly

**Requirement already satisfied**

Check the contents of the `tensorflow` package in Anaconda Prompt:

```
conda list tensorflow
```

Should return something like:

 Name    |                Version    |               Build | Channel
 ----|--|--|--
tensorflow    |            1.10.0      |              <pip>|
tensorflow      |          1.1.0         |      np112py36_0|
tensorflow-tensorboard  |  1.5.1        |             <pip>|

Check the contents of tensorflow using Pip

```
pip show tensorflow
```
Running the above command will return the following:

> Name: tensorflow <br>Version: 1.10.0 <br>Summary: TensorFlow is an open source machine learning framework for everyone.
<br>Home-page: https://www.tensorflow.org/
<br>Author: Google Inc.
<br>Author-email: opensource@google.com
<br>License: Apache 2.0
<br>Location: c:\users\akshi\anaconda3\lib\site-packages
<br>Requires: setuptools, numpy, wheel, termcolor, absl-py, astor, gast, grpcio, protobuf, tensorboard, six

## Troubleshooting and Gotchas!

* Make sure you are using the right version of Numpy with TensorFlow
  - `numpy<=1.14.5 >=1.13.3`
  - higher version of numpy could be incompatible with tensorflow and older version may not meet package requirements
* Delete older version of numpy using,
```
pip uninstall numpy
```
* To upgrade `numpy` run the following_path
```
pip install -U numpy
```

* While running the scripts if tensorflow_hub cannot be found then install it explicitely
```
pip install tensorflow_hub
```
