# ios-pipeline

## Github Secrets

- You'll need to setup a user with an SSH key to be able to pull a separate match repository
- Then configure the below environment variables

```
APP_STORE_CERT_NAME={your certificates common name}
APP_STORE_CONNECT_API_KEY_KEY_ID={API_KEY}
APP_STORE_CONNECT_API_KEY_ISSUER_ID={ISSUER_ID}
APP_STORE_CONNECT_API_KEY_IS_KEY_CONTENT_BASE64=true
APP_STORE_CONNECT_API_KEY_KEY={content of the .p8 file base64 encoded}
CERTS_SSH_PRIVATE_KEY={the private key to access your certificate repo}
FASTLANE_TEAM_ID={TEAM_ID}
KEYCHAIN_PASSWORD={A Password for the temp keychain your build lane will create}
MATCH_PASSWORD={the password used to encrypt your certificates repo}
```