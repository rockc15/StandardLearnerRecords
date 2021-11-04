# Standard Learner Records 
Program API Version 1.0

## Required Software
1. Node js


## How to Run the Server

1. Download All the Dependencies 
```bash
npm i
```

2. Run the Server
```bash
npm start
```


## How to Write to the Learner Records
1. Send a PUT request to `http://3.132.12.204:4000/writeToLearnerRecord`
2. The Body of the PUT  request will be a JSON object with this structure:

```JSON
Request.Body = {"triples":"the cco triples that will be uploaded"}
```

> NOTE: For the first iteration will will provided you with the JSON object needed for the BODY

## How to Read from the Learner Records

1. Send a GET request to `http://3.132.12.204:4000/readLearnerRecord/${query}/${playerID}`
2. Where  `${playerID}`  = SystemInfo.deviceUniqueIdentifier
3. Where  `${query}` = On of these strings “words”, “Letters”
