![Airbnb](http://www.underconsideration.com/brandnew/archives/airbnb_logo_detail.png "Airbnb")

Airbnb REST API (Unofficial)
============================

[Airbnb](https://www.airbnb.com/) API for retrieving
> unique accommodations from local hosts in 190 countries

*Note: This is an unofficial API and not supported or controlled by Airbnb itself. Any questions, comments, feedback or feature requests should be directed to [@tejas-manohar](https://github.com/tejas-manohar) or via an [issue](https://github.com/tejas-manohar/airbnb/issues/new) in this repo.*

Usage
=====

**Base URL:** http://airbnb-api-tm.herokuapp.com/

**Parameters:**
- loc (location)
- in (check in)
- out (check out)
- ppl (guests)

Dates are in the format of MM/DD/YYYY with standard URL encoding (2F = /)

**Output:** JSON

#### `GET /search`

Example Query:

```
http://airbnb-api-tm.herokuapp.com/search?loc=nashville&in=10%2F14%2F2014&out=10%2F15%2F2014&ppl=2
```

Response:

```json
{
  "status": "success",
  "accomodations": [
    {
      "permalink": "/rooms/3571396",
      "title": "Cozy Private Room off Charlotte !!!",
      "description": "Grace Cottage is a wonderful 1920s home situated in the beautiful town of Washington,     Arkansas.The home comfortably fits four and is located next to Historic Washington State Park. Enjoy a relaxing and restful weekend in the community of Washington.",
      "image": "https://a1.muscache.com/pictures/51710849/large.jpg",
      "visibility": "private room",
      "guests": 2,
      "bedrooms": 1,
      "beds": 1,
      "reviews": {
        "count": 11,
        "stars": 5
      },
      "user": {
        "firstName": "Laurence",
        "userId": "17981042"
      },
    },
    ...
    ...
```
