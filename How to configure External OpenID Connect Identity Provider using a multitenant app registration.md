# power-pages-notes

## How to configure External OpenID Connect Identity Provider using a multitenant app registration
Refer to https://learn.microsoft.com/en-us/power-pages/security/authentication/openid-provider 

Now, use the following key-value pairs for Power Pages to be able to get the token from the multitenant app registration after logon.
* Authentication/OpenIdConnect/OpenId_1/Authority: https://login.microsoftonline.com/common/
* Authentication/OpenIdConnect/OpenId_1/IssuerFilter: https://login.microsoftonline.com/*/v2.0
* Authentication/OpenIdConnect/OpenId_1/MetadataAddress: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration
* Authentication/Registration/LoginButtonAuthenticationType: https://login.microsoftonline.com/common/

Add an issue if you have a question.
