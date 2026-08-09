# Manual API Testing with Postman

## Overview

This project contains manual API testing performed using **Postman**. I tested the Google Maps Place APIs and covered the basic CRUD operations: Create, Read, Update, and Delete.

## APIs Tested

| Operation    | Method | Endpoint                      |
| ------------ | ------ | ----------------------------- |
| Add Place    | POST   | `/maps/api/place/add/json`    |
| Get Place    | GET    | `/maps/api/place/get/json`    |
| Update Place | PUT    | `/maps/api/place/update/json` |
| Delete Place | DELETE | `/maps/api/place/delete/json` |

## Add Place – POST

Used to create a new place.

**URL:**

```text
https://rahulshettyacademy.com/maps/api/place/add/json?key=qaclick123
```

**Sample Request:**

```json
{
  "location": {
    "lat": -38.383494,
    "lng": 33.427362
  },
  "accuracy": 50,
  "name": "Frontline house",
  "phone_number": "(+91) 983 893 3937",
  "address": "29, side layout, cohen 09",
  "types": [
    "shoe park",
    "shop"
  ],
  "website": "http://google.com",
  "language": "French-IN"
}
```

I verified the response status and captured the `place_id` for the next requests.

## Get Place – GET

Used to retrieve the details of an existing place.

```text
https://rahulshettyacademy.com/maps/api/place/get/json?place_id={place_id}&key=qaclick123
```

The `place_id` is taken from the Add Place response.

## Update Place – PUT

Used to update an existing place.

```text
https://rahulshettyacademy.com/maps/api/place/update/json?key=qaclick123
```

**Sample Request:**

```json
{
  "place_id": "{place_id}",
  "address": "70 Summer walk, USA",
  "key": "qaclick123"
}
```

After updating, I used the Get Place API to verify that the changes were reflected.

## Delete Place – DELETE

Used to delete an existing place.

```text
https://rahulshettyacademy.com/maps/api/place/delete/json?key=qaclick123
```

**Sample Request:**

```json
{
  "place_id": "{place_id}"
}
```

After deletion, the Get Place API can be used to verify that the place is no longer available.

## Testing Covered

* CRUD operations
* Request and response validation
* HTTP status code validation
* Query and path parameters
* JSON request/response validation
* Positive test scenarios
* Negative test scenarios

## Tools

* Postman
* REST API
* JSON
* Git
* GitHub

## Project Structure

```text
Manual-API-Testing-Postman/
│
├── postman/
│   └── Manual_API_Testing.postman_collection.json
│
└── README.md
```

## Author

**Archana**
QA Engineer | Automation & API Testing

[GitHub](https://github.com/Archana4GitHub)
