# Error Message

## Template

* HTTP 200 OK

```json
{
  "message": "OK",
  "data": [{
    "field1": "asd",
    "field2": ["asd", "asd"]
  }]
}
```

* HTTP 403 404 500

```json
{
  "message": "asdasd",
  "errors": [{
    "field1": "err",
    "field2": "err2"
  }]
}
```

```json
{
  "message" : "err"
}
```
