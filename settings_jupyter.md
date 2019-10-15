## Jupyter

The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.
Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more.

Is the default tool for this lab and it's one of the common tools for Data Science used worldwide.

Jupyter is installed by default inside the base conda environment, but if you want to use inside your new conda virtual environment you have to install on it.

To install jupyter inside conda you have to:
1. activate your conda venv
2. launch `conda install jupyter`
3. run jupyter typing `jupyter notebook`

Everytime you want to launch Jupyter notebook with your custom conda virtual environment you have to:
1. activate your conda env
2. run: `jupyter notebook` inside the terminal

then a new browser window will appear and you can use Jupyter from there with your venv.

If you want to close jupyter
1. save your work
2. close the browser tabs
3. press: CRTL + C inside the console windows to kill all the kernels and jupyter server

#### Set Jupyter default project folder

You can set the default Jupyter home main folder with this simple guide

Use the jupyter notebook config file:  
After you have installed Anaconda..
1. Open cmd (or Anaconda Prompt) and run jupyter notebook --generate-config.  
2. This writes a file to C:\Users\username\.jupyter\jupyter_notebook_config.py.  
3. Browse to the file location and open it in an Editor  
4. Search for the following line in the file: #c.NotebookApp.notebook_dir = ''  
5. Replace by c.NotebookApp.notebook_dir = '/the/path/to/home/folder/'  
6. Make sure you use forward slashes in your path and use /home/user/ instead of ~/ for your home directory, backslashes could be used if placed in double quotes even if folder name contains spaces as such :  "D:\yourUserName\Any Folder\More Folders\"  
7. Remove the # at the beginning of the line to allow the line to execute  