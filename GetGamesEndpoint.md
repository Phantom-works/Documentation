# API Endpoints - Adviser GetGames API

The following documentation provides information about the API endpoints available in the Adviser GetGames API microservice.

## Endpoint: POST /Games

This endpoint allows you to retrieve a list of games based on the specified genres.

### Request

- HTTP Method: POST
- URL: /Games

#### Request Body

The request body should be a JSON object with the following properties:


| Property | Type   | Required | Description                                         |
|----------|--------|----------|-----------------------------------------------------|
| genres   | Array  | Yes      | An array of genre slugs. Example: ["action", "rpg"] |

*example:* 

```json
{
"genres": ["action", "rpg"]
}
```

### Response

- HTTP Status Code: 200 (OK)
- Content-Type: application/json

#### Response Body

The response body will be a JSON array containing the game objects with the following properties:

| Property | Type   | Description                         |
|----------|--------|-------------------------------------|
| name     | String | The name of the game.               |
| cover    | Object | An object containing the URL of the game's cover image. |
| url      | String | The URL of the cover image.         |


*example:*

HTTP/1.1 200 OK

Content-Type: application/json

```json
[
  {
    "name": "Game 1",
    "cover": {
      "url": "https://example.com/game1.jpg"
    }
  },
  {
    "name": "Game 2",
    "cover": {
      "url": "https://example.com/game2.jpg"
    }
  }
]

# Error Responses

If the request body is missing the genres property, the API will respond with a 400 (Bad Request) status code.
Example Error Response



HTTP/1.1 400 Bad Request

```json
{
  "message": "Genres are required."
}
```
