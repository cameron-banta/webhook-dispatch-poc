# webhook-dispatch-poc

## POC to use nginx+lua to route webhooks based on json body field
Copy `mapping.sample` to `mapping`
Start the stack, and http/curl/etc to http://localhost:8080
```
http POST http://localhost:8080 OrganizationId=org1
http POST http://localhost:8080 OrganizationId=org2
http POST http://localhost:8080 OrganizationId=bogus
```

Check the results on http://localhost:8081 and http://localhost:8082

