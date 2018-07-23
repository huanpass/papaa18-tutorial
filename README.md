# PAPAA'18 Tutorials

These are the tutorials prepared by Professor Wayne Luk from Imperial College London to introduce the principles and usage of the Convolutional Neural Network (CNN) on Field Programmable Gate Arrays.

## Structure

The structure of the tutorials is:

_Session A_

-   [Tutorial 1](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/01%20Introduction%20to%20CNN%20and%20TensorFlow.ipynb): TensorFlow basics
-   [Tutorial 2](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/02%20Build%20CNN%20in%20DFG%20IR.ipynb): Data-Flow Graph IR and TensorFlow model parser

_Session B_

-   [Tutorial 3](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/03%20Fixed-Point%20Quantisation%20of%20CNN.ipynb): CNN quantisation effect and exploration
-   [Tutorial 4](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/04%20Deploy%20DFG%20IR%20on%20FPGA.ipynb): Hardware design generation and deployment

```bash
.
├── data
│   ├── figs
│   └── mnist_model
└── notebooks  # Here are the tutorials
    └── Answer # Here are the answers, please look after attempting ;)
├── model      # Here should be the checkpoint and model files
   └── ssd_ckpt
```

## Installation & Requirements

### Step #1: VirtualBox

We will need to install a Virtual Machine, in case you are not familiar here is the process:

#### Step #1.1: Download VirtualBox

Please navigate to this address and choose your distribution: <https://www.virtualbox.org/>.

#### Step #1.2: Install VirtualBox

Depending on your distribution please install VirtualBox.

### Step #2: Creating a VirtualMachine

#### Step #2.1: Download the installation disc

Please downlaod the image file `papaa-tutorial.ova`. This image has all dependencies preinstalled and is ready to use. Download it at: <https://s3-ap-southeast-1.amazonaws.com/corerain/PAPAA-tutorialWL.ova>. Or use BaiDuYun <https://pan.baidu.com/s/1A2barVEPNhvtUW1eR6gnjA>.

#### Step #2.2: Creating and booting up your VirtualMachine

Inside VirtualBox click on File -> Import Appliance and find the downloaded image on your disk and add it to the menu and then click Continue. All the settings that you are going to see in the next screen are pre-made, you just have to click Import. That should then take approximately 5-10 minutes or less depending on your machine.

##### Step #2.2.1: Power it up

Double click the imported machine to power it on and there we go!

We will be mostly using python in our demonstration. In case you are not familiar with python, check out this link which is doing a very good job at explaining the basics: [Link](https://learnxinyminutes.com/docs/python/).

### Step #3: Launching the Tutorials

```shell
# To get to the tutorial folder, or follow the alias link on your desktop
cd /home/jack/papaa18-tutorial/

# Activate the virtual environment
source venv/bin/activate

# To launch the jupyter notebook
jupyter notebook

# You should see an URL appear in the terminal if your browser automatically
# does not turn on copy that URL to your browser of choice
```

If you would like to install jupyter notebooks to run on your personal devices simply do:

```shell
# Assuming that you have pip installed
pip3 install --upgrade pip
pip3 install jupyter
```

## Contact

If you would like to discover more please do not hesitate to contact us at:

-   Professor Wayne Luk (w.luk@ic.ac.uk)

-   Martin Ferianc (martin.ferianc@corerain.com)

-   Ruizhe (Vincent) Zhao (vincent.zhao@corerain.com)
