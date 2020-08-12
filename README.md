# cloud-run-helloworld
Try Cloud Run

- Reference
  - https://cloud.google.com/run/docs/quickstarts/build-and-deploy?hl=ja#python


## Setup
```
$ git clone git@github.com:tayutaedomo/cloud-run-helloworld.git
$ cd cloud-run-helloworld
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install --upgrade pip
$ pip install -r requirements.txt
```


## Local Server
```
$ cd cloud-run-helloworld
$ source venv/bin/activate
$ python app.py
$ open 'http://0.0.0.0:8080/'
```
Open "http://0.0.0.0:8080/" with Web Browser.


## Build and Deploy
```
$ gcloud builds submit --tag gcr.io/[PROJECT-ID]/helloworld
$ gcloud run deploy --image gcr.io/[PROJECT-ID]/helloworld --platform managed
```

