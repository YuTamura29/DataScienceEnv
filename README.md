# What is this
If you need to compose up anaconda enviroment in docker, you can use this repository.
We can add any python library.

# How to use
## Step1: Clone
Clone this repository

## Step2: Add library 
If you some libirary, you should fix DockerFile.
Add some pip code.

```
RUN pip install -U pip && \
    pip install --upgrade setuptools && \
    pip install autopep8 && \
    pip install flake8 pycodestyle_magic --ignore-installed --user &&\
    pip install tensorflow --ignore-installed --user && \
    pip install opencv-python && \
    pip install tqdm
```

## Step3: Build and Run
Please use docker-compose up on directory of docker-compose.yml.
You can use any file under the directory.

## Step4: Start jupyter lab
Please copy jupyter-lab URL and paste the URL to search bar
