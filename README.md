# cloud-run-helloworld
Try Cloud Run


## Reference
- https://cloud.google.com/run/docs/quickstarts/build-and-deploy?hl=ja#python


## Build and Deploy
```
$ gcloud builds submit --tag gcr.io/[PROJECT-ID]/helloworld
$ gcloud run deploy --image gcr.io/[PROJECT-ID]/helloworld --platform managed
```

