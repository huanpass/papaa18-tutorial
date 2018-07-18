# PAPAA'18 Tutorials

These are the series of tutorials prepared by Professor Wayne Luk from Imperial College London to introduce the principles and usage of the Convolutional Neural Network (CNN) to Field Programmable Gate Arrays flow first introduced by Corerain Technologies Ltd..

## Installation

For this tutorial python3 is a must if you don't have it on your distribution please follow these links: [Linux](https://docs.python-guide.org/starting/install3/linux/), [Mac OSX](https://docs.python-guide.org/starting/install3/osx/) and [Windows](https://docs.python-guide.org/starting/install3/win/).

If you have access to our `plumber` repository, you may install and run the notebook on your own laptop.

```shell
git clone https://github.com/corerain/papaa18-tutorial $PAPAA18_TUTORIAL_DIR

git clone --recursive https://github.com/corerain/plumber $PLUMBER_DIR
cd $PAPAA18_TUTORIAL_DIR
virtualenv -p python3 venv
source venv/bin/activate

# Install plumber
pip install -e $PLUMBER_DIR
```

You might also need to install jupyter notebooks to run our tutorials and little exercises:

```shell
# Assuming that you have pip installed
pip3 install --upgrade pip
pip3 install jupyter
```

The whole process of installation (in case you are having problems) is [here](https://jupyter.readthedocs.io/en/latest/install.html).

## Contact

If you would like to discover more please do not hesitate to contact us at:

-   Professor Wayne Luk (w.luk@ic.ac.uk)

-   Martin Ferianc (martin.ferianc@corerain.com)

-   Ruizhe (Vincent) Zhao (vincent.zhao@corerain.com)
