# OneSphere example-app

This example makes use of the oidc package to fetch an access token for OneSphere  client ID. It requires a client ID and secret of a registered OAuth2 application in OneSphere.

1. Set the following environment variables with client ID and client secret.

```
ONESPHERE_CLIENT_ID=example-app
ONESPHERE_CLIENT_SECRET=ZXhhbXBsZS1hcHAtc2VjcmV0
OIDC_ISSUER=https://identity-next.dev.hpedevops.net/dex
```

2. Run the example and navigate to http://127.0.0.1:9999.

```
go run server.go
```
You will be prompted to login via the provider if you have not done so already. If the login in successful the API will send a response containing the access token to the example application which will be displayed.

For token validation, see LINE 70:server.go
