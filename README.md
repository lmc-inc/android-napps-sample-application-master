# Android Native Application SSO Sample Application

**android-napps-sample-application** is a basic sample application to demonstrate using the new Chrom Custom Tabs support in Android to facilitate native application single sign-on.

This sample application will authenticate the user via OpenID Connect 1.0 and present the user's subject and tokens on the screen. Options to refresh the OAuth 2.0 access token and to retrieve additional profile information via the Userinfo endpoint are also demonstrated.

Refer to the **Mobile Application SSO Developers Guide** at https://developer.pingidentity.com/en/resources/napps-native-app-sso for more detailed information.


## Installation

This sample application has been built using PingFederate 8.0.1 and the OAuth Playground 3.2. Follow the documentation for PingFederate and the OAuth Playground to quickly stand up an OpenID Connect Provider / OAuth Authorization Server.

Modify the OAuth client "ac_client" in the PingFederate configuration (OAuth Settings -> Client Management -> ac_client -> Redirect URIs) to include the application callback URI (com.pingidentity.developer.napps://oidc_callback) defined in the "strings.xml" file.

Modify the "Constants" file with the URL of your PingFederate server and the name of your issuer.


## Disclaimer

*This software is open sourced by Ping Identity but not supported commercially as such. Any questions/issues/comments should be directed to the "Developer Q&A" group in the Ping Identity Support Communities https://community.pingidentity.com/collaborate.*
