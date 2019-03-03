# Set cors to Firebase storage

I learned that we can set cors to Firebase storage.  
I investigated this because my app on Firebase hosting loads image files which can be taken from Firebase storage and domains are different.

## Tool
* Google Cloud SDK

## How to

0. Install Google Cloud SDK

https://cloud.google.com/sdk/

1. Initialize Google Cloud SDK
```shell
gcloud init
```

2. Create `cors.json`
```javascript
[{
  "origin": ["https://xxxx.firebaseapp.com", "http://localhost:3000"],
  "responseHeader": ["*"],
  "method": ["GET"],
  "maxAgeSeconds": 86400
}]
```

3. Deploy `cors.json`
```
gsutil cors set cors.json gs://xxxx.appspot.com 
```

4. Make sure your setting
```
gsutil cors get gs://xxxx.appspot.com 
```
