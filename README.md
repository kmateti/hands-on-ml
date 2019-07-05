# hands-on-ml
Going through the Hands-On Machine Learning book, plus applying it to other interesting datasets.

# Setup

While one could install Anaconda, or Miniconda, I am trying to do a minimalist install with just ```pip```, and the book goes through this nicely.  I am copying most of this from the book.
## ```python``` Installation
In either Windows or Linux, we need to make sure python3 is installed.  First just try to see what typing ```python``` or ```python3``` into the command line does.

If you see Python 3.x.x show up you are good, like this
```
PS C:\dev\hands-on-ml> python
Python 3.7.1 (v3.7.1:260ec2c36a, Oct 20 2018, 14:05:16) [MSC v.1915 32 bit (Intel)] on win32
```
## ```pip``` Installation
Check your pip version
```
PS C:\dev\hands-on-ml> python -m pip --version
pip 19.1.1 from C:\Python37-32\lib\site-packages\pip (python 3.7)
```

```pip``` should be installed by default since Python 2.7.9, but if it is not, you will have to google fu.

Upgrade pip by
``` python -m pip install --upgrade pip```

## ```virtualenv``` Installation

It is best practice to use virtual environments to isolate library dependencies. 

```
$ python -m pip install virtualenv
```

### Create a virtual environment

```
cd ~/ml
virtualenv env
```

### Install Required Modules

```
python -m pip install jupyter matplotlib numpy pandas scipy scikit-learn
```

Check the installation by running the following, there should be no output or errors.

```
python -c "import jupyter, matplotlib, numpy, pandas, scipy, sklearn"
```