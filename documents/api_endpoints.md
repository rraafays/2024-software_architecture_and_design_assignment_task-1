# API Endpoints

## Media Items

**Endpoint**: GET /api/media-items
**Description**: gets all media items

**Headers**:

- Content-Type: application/json; charset=utf-8

***Response***:

- HTTP/1.1 200 OK

```json
{
    "data": [
        {
            "author": "Ridley Scott",
            "availability": 10,
            "createdAt": "2024-12-17T11:46:51.904Z",
            "documentId": "meloko8lya1nuream9zl4ln2",
            "format": "Movie",
            "genre": "Cyberpunk",
            "id": 4,
            "publishedAt": "2024-12-17T11:46:56.357Z",
            "title": "Blade Runner",
            "updatedAt": "2024-12-17T11:46:56.352Z"
        },
        {
            "author": "Bandai Namco Games",
            "availability": 13,
            "createdAt": "2024-12-13T22:31:19.238Z",
            "documentId": "ixkrv77v4v9qd9u265rn26co",
            "format": "Video Game",
            "genre": "Fighting",
            "id": 5,
            "publishedAt": "2024-12-17T11:47:12.908Z",
            "title": "TEKKEN 8",
            "updatedAt": "2024-12-17T11:47:12.904Z"
        }
    ],
    "meta": {
        "pagination": {
            "page": 1,
            "pageCount": 1,
            "pageSize": 25,
            "total": 2
        }
    }
}
```
