# Developing a RESTful API with Go and Gin

> the basics of writing a RESTful web service API with Go and the Gin Web Framework (Gin).

## Install Dependencies

```
go get .
go get: added \
    github.com/gin-gonic/gin v1.7.2
```

## Start Service

```
go run .

```

## getAlbums (/albums)

- GET – Get a list of all albums, returned as JSON.

````
> curl to make a request to your running web service.

curl http://localhost:8080/albums
`````

## postAlbums (/albums)

- POST – Add a new album from request data sent as JSON.

````
curl http://localhost:8080/albums \
--include --header \
"Content-Type: \
application/json" --request \
"POST" --data '{"id": \
"4","title": "The Modern Sound \
of Betty Carter","artist": \
"Betty Carter","price": 49.99}'
````

## getAlbumByID (/albums/:id)

- GET – Get an album by its ID, returning the album data as JSON.

````
curl http://localhost:8080/albums/2
````

