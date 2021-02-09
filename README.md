# Progress Plus Application

Hello and welcome to the back end of our Application **Progress Plus**.

This was made by the combined efforts of **Charlie Chandler**, **Freshta Ebrahim**, **Hajoo Chung**, **Ionut Predoi**, **Ismail Ali** and **Patrick Fleming**.

This is a platform to allow School of Code bootcampers and coaches to track the technical progress of bootcampers.  Coaches can register, submit written feedback, and compare the progress of bootcampers and the bootcamp as a whole.  Bootcampers can register and view their scores and written feedback for the various mastery and recap tasks they complete.

Here is the [deployed version](http://3.250.192.68:3000/), which is hosted in a cluster on AWS's Elastic Container Service. 

You can find the client code [here](https://github.com/patrickjfl/progress-plus-client).

## Stack

- `Node JS`
- `Express`
- `Firebase`
- `Docker`
- `Postgres`

## Getting started

1. Clone the repo: `git clone https://github.com/patrickjfl/progress-plus-server.git`

2. Download the required npm modules: `npm i`

## Useful commands

- `npm start` - run the server

## ---- Routes ----

All routes use a middleware function that checks their firebase authentication, If they fail the check, they are returned the message
_You are not authorized to make this request_

### GET to /

Returns to successful requests in the from:

```
```

### GET to /

Returns to successful requests in the from:

```
```

### GET to /feedback

Returns to successful requests in the from:

```
{success: true,
data: 
  [{"uid": "d6587569589dk3r437890584gjfni",
  "duedate": "2020-11-15T00:00:00.000Z",
  "datesubmitted": "2020-11-15T00:00:00.000Z"}, ... ]}	

The elipses represent more objects with the same keys.	
```



Firstly checks if there is a uid query, if there is then it will execute next() and move on to the next middleware function.
