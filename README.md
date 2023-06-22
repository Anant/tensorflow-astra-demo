# DataStax AI Tutorials Series: Tensorflow & AstraDB Quickstart

Use your Astra Database to store your data and model.

The Astra DB & TensorFlow repository demonstrates how to seamlessly integrate Astra DB, a highly scalable and cloud-native database, with TensorFlow, a popular deep learning framework. This integration enables developers to harness the power of Astra DB's distributed data storage and retrieval capabilities while leveraging TensorFlow's advanced machine learning and deep neural network functionalities.

By combining Astra DB's flexible data modeling, automatic scaling, and global distribution features with TensorFlow's robust capabilities for training and deploying deep learning models, this integration provides a comprehensive solution for building scalable and high-performance machine learning applications.


## Setup

### Clone the Repo
To get started, you need to get the code onto your machine. So Start by cloning this GitHub repository. If you have git installed, you can do this by running the following command in your terminal:

```bash
git clone git@github.com:Anant/tensorflow-astra-demo.git
```

This will create a copy of the repository on your local machine.
Once you have cloned the repository, navigate into the directory:

```bash
cd tensorflow-astra-demo
```
### Install Prerequisites

To install the required packages for this plugin, run the following command:

```bash
pip install -r requirements.txt
```

### Setup A DataBase

In order to run the examples from this repo, you will need to set up a database and create a keyspace.
The details of how to do this should be found under the following link
<link>

### Setup the DataBase Details

Once you've got the database up and running and the keyspace created, make sure you download the bundle as described in the link above and get the keys needed to access your database.
Now open the local_secrets.py file and make sure you fill  in the details
```
client_id="<your-client_id>"
client_secret="<your-client_secret>"
token="<your-token>"
db_keyspace="<your-keyspace>"
secure_bundle_path="<path-to-bundle>/secure-connect-tensorflow-demo.zip"
```

### Install jupyter lab

One important tool we will use here for an interactive coding is jupyter lab, or jupyter notebooks as well.  
Jupyter lab in particular has more advanced functionalities than traditional notebooks. So if you don't have jupyter locally feel free to install the labs feature using the following command.

```
pip install jupterlab
```

### Run the notebooks

After installing the jupyterlab, go to the terminal, inside your working directory (or the directory you cloned as per the instructions above) and run the following command:

```
jupyterlab
```
This should redirect you to the browser automatically, if not you should be able to see the instructions on how to navigate to the jupyter env on the terminal itself. 


Now you can start running the steps from the notebook (executing the cells in order), to run the code that populates and extracts data from your AstraDB tables.
The description of this can be found in the following link <link to the blog>.


**Note**

For this example the version of python used is: 3.10.11 

As for the data, you will find a sample data under the data folder in this repository but feel free to use any dataset with the same schema. 
