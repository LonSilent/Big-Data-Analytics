# Big-Data-Analytics
### IPython Notebook with spark install 

### Install Anaconda (iPython)
```
wget http://repo.continuum.io/archive/Anaconda2-4.0.0-Linux-x86_64.sh
bash Anaconda2-4.0.0-Linux-x86_64.sh
conda install jupyter
```
### Install Jupyter notebook
```
sudo apt-get update
sudo apt-get install python-pip python-dev build-essential
sudo pip install --upgrade pip
sudo pip install “ipython[notebook]”
jupyter notebook
```

### link Spark
```
sudo vim ~/.bashric
export PYSPARK_DRIVER_PYTHON=ipython
export PYSPARK_DRIVER_PYTHON_OPTS='notebook' pyspark
source ~/.bashrc
pyspark
```
### pyspark csv
```
pyspark --packages com.databricks:spark-csv_2.10:1.4.0
```
