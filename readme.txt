Installing software
-------------------

Machines in lab G24 and various overflow labs should have all the necessary software already installed. 

But here are some notes for running on your own machine.

I will be running under Linux and using Python 3; see http://www.python.org

I shall also be using the following:
    
1) Jupyter from https://jupyter.org/ 

2) the Python package pandas; see http://pandas.pydata.org/

3) The Python package scikit-learn (sklearn), which in its turn requires numpy, scipy and a number of other things; see http://scikit-learn.org/

4) The Python package matplotlib from http://matplotlib.org/

One way to get everything you need is to install Anaconda: https://www.continuum.io/downloads

You'll need to use a modern browser: Chrome will do. Set it as your default browser: it will be launched whenever you
start the notebook server. Furthermore, if it uses a proxy, you'll need to bypass the proxy for requests to localhost.
Bring up the dialogue box for changing the proxy, and either set it to no proxy (but this means you won't be able to
use the web while running the notebook) or specify 127.0.0.1 and localhost as *exceptions* to the proxy.

Please share with me and the class any update or variations to these notes, e.g. instructions for installing on Windows.

Running software
----------------

Resources that you download from the module web site will unpack to a directory called CS4619Resources. Within this
directory, you'll find lecture notes, images used within the notes, datasets (as CSV files), and so on.

The lecture notes come in the form of Jupyter notebooks.

To open a Jupyter notebook: change to the directory that I mentioned above and then type

> jupyter notebook

This starts a local server and opens your default web browser at the Jupyter application dashboard. From there, you can choose a notebook to open.

After you've opened a notebook, it's often a good idea to choose Run All Cells from the toolbar so that all the code in the 
notebook runs.

The notebook consists of cells. You can insert new cells into the notebook from the toolbar. By default, new cells will be Code cells, into which you can type Python. But you can change them to Markdown cells from the toolbar, into which you can type text with markup. In all cells, hitting Enter inserts a new line into the cell. But hitting Shift-Enter executes the cell. This executes the Python in Code cells or renders the markup in Markdown cells.

Don't forget to save notebooks that you create, although they are autosaved at regular intervals.

We will use the first few Code cells in every notebook to set things up. In particular, one of these cells will contain the 
following:

%matplotlib inline

which means that graphs that we draw will be rendered within the notebook, rather than in a separate window.

Another of these cells will also include some Python import statements.
