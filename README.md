# ggplot2-book

Repository for coding examples of ggplot2 following [ggplot2: Elegant Graphics 
for Data Analysis](https://ggplot2-book.org/index.html).  Below are instructions
on how to set up the R kernel for Jupyter Notebook which enables an interactive
plotting environment.

## Setting up the Jupyter Notebook
1.  Download Miniconda3 from https://docs.conda.io/en/latest/miniconda.html.  
This repo downloaded the [Miniconda3 Windows 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-py39_4.9.2-Windows-x86_64.exe), 
which contains python v3.9 and conda v4.9.2

2.  Update to the newest version
	```cmd
	(base) C:\Users\jab112> conda update conda
	
	(base) C:\Users\jab112> conda --version
	conda 4.10.1
    ```

3.  Create the conda environment
	```cmd
	(base) C:\Users\jab112> conda create --name ggplot2-book
	
	# Add the conda-forge conda channel
	(base) C:\Users\jab112> conda config --add channels conda-forge
	
	(base) C:\Users\jab112> conda config --show channels
	channels:
	  - conda-forge
	  - defaults
	  
	(base) C:\Users\jab112> conda activate ggplot2-book
	
	(ggplot2-book) C:\Users\jab112> 
	```

4.  Install R (v4.0.3) and Jupyter
    ```cmd
	(ggplot2-book) C:\Users\jab112> conda install r-base=4.0.3
	
	(ggplot2-book) C:\Users\jab112> conda install jupyter
	
	# Initiate an R session to install the required packages
	(ggplot2-book) C:\Users\jab112> R

    ```	

5.  Install the `IRkernel` package
	```R
	> install.packages("IRkernel")
	
	> IRkernel::installspec()
	```

5.  Start the Jupyter Notebook
	```cmd	
	(ggplot2-book) C:\Users\jab112> jupyter notebook
	```
