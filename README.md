# Big-Data-Analytics
## IPython Notebook with spark install 

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

## link with AWS
### login cluster
```
ec2/spark-ec2 -k bigdata -i bigdata.pem -r us-west-2 login cluster
```
### run pyspark with AWS
```
./bin/pyspark --master spark://ec2-52-40-241-52.us-west-2.compute.amazonaws.com:7077
```
### Notice! You should export AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY in your shell, and bigdata.pem is necessary, please PM me if you want.
