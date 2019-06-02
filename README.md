* Keycloak server running at 8080

* import realm config from doc/realm-export.json

* create user in keycloak set password

* Under user - role mapping select client and add appropriate role

* Get bearer token using postman and user created refer following link to get token

* doc/getBearerToken.JPG

* use curl command like following to get resource


```
curl -X GET \
  http://localhost:8085/api/v1/employees/username \
  -H 'Accept: */*' \
  -H 'Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5' \
  -H 'Cache-Control: no-cache' \
  -H 'Connection: keep-alive' \
  -H 'Host: localhost:8085' \
  -H 'Postman-Token: 0d0f6ceb-1810-4233-bbb5-5e2058d8c1ef,47bc7de0-95f9-49f1-a288-679769663100' \
  -H 'User-Agent: PostmanRuntime/7.13.0' \
  -H 'accept-encoding: gzip, deflate' \
  -H 'cache-control: no-cache'
```

