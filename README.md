# go-url-shortener
## Run

Run with Docker

```bash
docker-compose up -d
```
## Code Example
Using CURL
### Generate shortener
```
$ curl --location 'http://localhost:3000/api/v1' \
--header 'Content-Type: application/json' \
--data '{
    "url":"https://www.youtube.com/watch?v=3ExDEeSnyvE&ab_channel=AkhilSharma"
}'
```
### Response:
```
{
    "url": "https://www.youtube.com/watch?v=3ExDEeSnyvE&ab_channel=AkhilSharma",
    "short": "localhost:3000/4758ec",
    "expiry": 24,
    "rate_limit": 9,
    "rate_limit_reset": 30
}
```

Redirect
Open URL in your browser [http://localhost:3000/4758ec](url)
