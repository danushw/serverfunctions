# Google cloud Functions Course

Maran Hagevet

## Starting a projectas

Why 1 day like that

### 3 Hash

To start a new project in google cloud, we can go to the [Firebase Console](https://console.firebase.google.com) or create it from [Google Cloud Platform Console](https://console.cloud.google.com)

## Creating a virtual environment

First we have to install 'python3-venv' with:

## Windows

Taken from this [Link](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)

```
py -m pip install --user virtualenv
```

To activate the Virtual Environment we do:

```
.\env\Scripts\activate
```

for fixing a problem-

```
pip install wheel
```

in PyCharm-
File > Settings > Project > Python Interperter -
Add Interperter -
Existing Environment

## Linux

```
sudo apt install python3-venv
```

## Deplyoing our function

FIrst, we have to set our project ID with the following command

```
gcloud config set project [YOUR_PROJECT_ID]
```

Then we deploy our function with this command:

gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
