# papaa18-tutorial
Tutorials for the PAPAA '18 summer school

## Install

If you have access to our `plumber` repository, you may install and run the notebook on your own laptop.

```shell
git clone https://github.com/corerain/papaa18-tutorial $PAPAA18_TUTORIAL_DIR

git clone --recursive https://github.com/corerain/plumber $PLUMBER_DIR
cd $PAPAA18_TUTORIAL_DIR
virtualenv -p python3 venv
source venv/bin/activate

# install plumber
pip install -e $PLUMBER_DIR
```
