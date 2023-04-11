# webhook-dispatch-poc

## POC to use nginx+lua to route webhooks based on json body field
To run this poc, start the stack (`docker compose up`) then browse to 
http://localhost:8081 and http://localhost:8082 and get the UUIDs for each. 
Replace the values in `default.conf.template` (lines 6 and 7)

Restart the stack, and http/curl/etc to http://localhost:8080
```
http POST http://localhost:8080 OrganizationId=org1
http POST http://localhost:8080 OrganizationId=org2
http POST http://localhost:8080 OrganizationId=bogus
```
