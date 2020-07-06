# Proof-of-Concept OpenID Connect Provider

This is just a simple POC for OpenID Connect provider implementation to log user in.

Created for a quick demo purpose. Has only one user.

# Usage

```bash
yarn install
node server.js
```

# URLs

| URL                      | Description                                       |
| ------------------------ | ------------------------------------------------- |
| `GET /oauth2/authorize`  | Login form                                        |
| `POST /oauth2/authorize` | Check user credentials + redirect to redirect URI |
| `POST /oauth2/token`     | The URL where ID token is fetched from            |

# Environment variables

| Name          | Default value      | Description                       |
| ------------- | ------------------ | --------------------------------- |
| PORT          | 3000               | Web server port                   |
| CLIENT_ID     | clientid0123456789 | OpenID Connect provider client ID |
| CLIENT_SECRET | secret0123456789   | OpenID Connect provider secret    |
| USER_LOGIN    | test               | User login                        |
| USER_PASS     | pass               | User password                     |
