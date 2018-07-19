# PAPAA'18 Tutorials

These are the series of tutorials prepared by Professor Wayne Luk from Imperial College London to introduce the principles and usage of the Convolutional Neural Network (CNN) to Field Programmable Gate Arrays flow first introduced by Corerain Technologies Ltd..

## Structure

The structure of the tutorial is:

_First session_

-   [Tutorial 1](<notebooks/01\ Introduction\ to\ CNN\ and\ TensorFlow.ipynb>): TensorFlow basics
-   [Tutorial 2](<notebooks/02\ Build\ CNN\ in\ DFG\ IR.ipynb>): Data-Flow Graph IR and TensorFlow model parser

_Second Session_

-   [Tutorial 3](<notebooks/03\ Fixed-Point\ Quantisation\ of\ CNN.ipynb>): CNN quantisation effect and exploration
-   [Tutorial 4](<notebooks/04\ Deploy\ DFG\ IR\ on\ FPGA.ipynb>): Hardware design generation and deployment

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

## Installation

### Step #1: VirtualBox

We will need to install a Virtual Machine, in case you are not familiar here is the process:

#### Step #1.1: Download VirtualBox

Please navigate to this address and choose your distribution: <https://www.virtualbox.org/>.

#### Step #1.2: Install VirtualBox

Depending on your distribution please install VirtualBox.

### Step #2: Creating a VirtualMachine

#### Step #2.1: Download the installation disc

Please downlaod this installation `.iso` disc depending on your system. Please choose one between `ubuntu-16.04.4-desktop-i386.iso` and `ubuntu-16.04.4-desktop-amd64.iso` from this site: <http://releases.ubuntu.com/16.04/>.

#### Step #2.2: Creating and booting your VirtualMachine

More detailed tutorial: <https://www.wikihow.com/Install-VirtualBox#step_4_1>

##### Step #2.2.1:

Inside VirtualBox, click New. This will open the wizard that will guide you through the process to create your virtual machine.

On the first screen of the wizard, you will be asked to give the new virtual machine a name as well as choose what operating system you will be installing. In our case it is going to be Linux.

If you are installing the 64-bit version of the operating system, make sure to choose the 64-bit version from the Version menu.

Click Continue. It's at the bottom of the window.

##### Step #2.2.2:

Set the amount of RAM. You will need to designate how much of your computer's RAM will be allocated to your virtual machine. VirtualBox will automatically choose the recommended minimum amount for the operating system you selected, but you can increase or decrease this if you'd like, but the default value should be ok for us.

Click Continue.

##### Step #2.2.3:

Create a virtual hard drive. Select a virtual hard drive option and click Create, then click through the prompts and click Create again.

The most common format for virtual hard drives is VDI (VirtualBox Disk Image), this one we will also use.

##### Step #2.2.4:

Storage on physical hard disk, please select Dynamically allocated.

##### Step #2.2.5:

File location and size. Please select where would you like to store the VDI for the purposes of the tutorial and select the size of how much it should take, for our purposes 10 GB is going to be enough, click Create.

##### Step #2.2.6:

Start the operating system installation. Once the virtual machine has been configured, the wizard will close and you will be taken back to the VirtualBox main window. Double-click your new machine in the left menu, then do: click the folder-shaped icon to browse through your computer for the installation image file.

Click Start. It's at the bottom of the window. This will prompt VirtualBox to begin reading our disk.

This image that we have downloaded and installed has all dependencies already pre-installed.

In case you are not familiar with python, check out this link which is doing a very good job at explaining the basics: [Link](https://learnxinyminutes.com/docs/python/).

For this tutorial python3 is a must if you don't have it on your distribution please follow these links: [Linux](https://docs.python-guide.org/starting/install3/linux/), [Mac OSX](https://docs.python-guide.org/starting/install3/osx/) and [Windows](https://docs.python-guide.org/starting/install3/win/).

If you have access to our `plumber` repository, you may install and run the notebook on your own laptop.

```shell
git clone https://github.com/corerain/papaa18-tutorial $PAPAA18_TUTORIAL_DIR

git clone --recursive https://github.com/corerain/plumber $PLUMBER_DIR
cd $PAPAA18_TUTORIAL_DIR
virtualenv -p python3 venv
source venv/bin/activate

# Install plumber
pip3 install -e $PLUMBER_DIR
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
