# cURL for RESTful API testing <sup>[[source]](http://blogs.plexibus.com/2009/01/15/rest-esting-with-curl)</sup>

Parameter | Description
--------- | -----------
-i        | show response headers
-H        | pass request headers to the resource
-X        | pass a HTTP method name
-d        | pass in parameters enclosed in quotes; multiple parameters are separated by '&'

## Examples

### PUT a resource

```
curl -i -H "Accept: application/json" -X PUT -d "phone=1-800-999-9999" http://192.168.0.165/persons/person/1
```

### GET a resource

```
curl -i -H "Accept: application/json" http://192.168.0.165/persons/person/1
```

### For GET requests, the -X GET option is optional

```
curl -i -H "Accept: application/json" http://192.168.0.165/persons?zipcode=93031
```

### You can pass in query parameters by appending it to the url

```
curl -i -H "Accept: application/json" http://192.168.0.165/persons?firstName=james&lastName=wallis
```

### DELETE a resource

```
curl -i -H "Accept: application/json" -X DELETE http://192.168.0.165/persons/person/1
```
