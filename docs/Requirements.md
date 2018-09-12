# Image Classification Workshop Requirements

For the workshop, please make sure you have the listed requirements installed. If you encounter issues other than mentioned in this document, reach out to us before the workshop starts.

## Installation Requirements

* Python
  - You can install Python by installing Anaconda using these [instructions](https://conda.io/docs/user-guide/install/index.html#regular-installation)

* `Bash` or `command prompt` to run scripts using Python
  - Windows users add python to environment variables, see this [example](https://medium.com/@GalarnykMichael/install-python-on-windows-anaconda-c63c7c3d1444)

* `Jupyter Notebook` or `Google Collab Notebook` (*optional*)

* You should have either `pip` or `Anaconda Prompt` installed to install the required packages:

  * **Option 1**: `pip`
    - Install `pip` on [Windows](https://github.com/BurntSushi/nfldb/wiki/Python-&-pip-Windows-installation), [Others](https://packaging.python.org/tutorials/installing-packages/)

  * **Option 2**: `Anaconda Prompt`
    - packages can be installed using anaconda prompt **which comes along the Anaconda distribution** if pip is not installed

* The following Python packages need to be installed:

  - `numpy` (version >=1.13.3)
  - `tensorflow`
  - `tensorboard`

  You can install Python packages using either `pip` or `anaconda prompt` (depending on what you have installed):

  If pip is already installed or you have `Anaconda` distribution of Python, run the following:

  ```
  pip install numpy
  pip install tensorflow
  pip install tensorboard
  ```

  Alternatively, for `anaconda prompt` run the following:

  ```
  conda install numpy
  conda install tensorflow
  conda install tensorboard
  ```

  `tensorboard` comes along with `tensorflow` so we might see the following while installing `tensorflow` explicitly

> **Requirement already satisfied**

You can check the contents of `tensorflow` in `anaconda prompt`:

```
conda list tensorflow
```

It should return something like this:

 Name    |                Version    |               Build | Channel
 ----|--|--|--
tensorflow    |            1.10.0      |              <pip>|
tensorflow      |          1.1.0         |      np112py36_0|
tensorflow-tensorboard  |  1.5.1        |             <pip>|

You can check the contents of `tensorflow` using `pip`:

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

## Troubleshooting during the workshop!

* Make sure you are using the right version of Numpy with TensorFlow
  - `numpy<=1.14.5 >=1.13.3`
  - higher version of `numpy` could be incompatible with `tensorflow` and older version may not meet package requirements.

* Delete older version of `numpy` using,

  ```
  pip uninstall numpy
  ```
  
* To install a specific version of `numpy`, use the following command:

  ```
  pip install numpy==1.14.5
  ```

* To upgrade `numpy` run the following:

  ```
  pip install -U numpy
  ```

* While running the scripts, if `tensorflow_hub` cannot be found then install it explicitely:

  ```
  pip install tensorflow_hub
  ```

* When re-training the model, if the windows users run into Permission errors, try deleting the troubling log file manually
