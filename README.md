These shell functions help you to use twitter api from `bash`.

## Installation

Sure, it has a one-liner installer:
```
curl -Lo /tmp/twitter-functions j.mp/twitter-functions && . /tmp/twitter-functions
```

## Obtaining Credentials

Navigate to the `API-keys` tab on the [Twitter Application](https://apps.twitter.com/) site.
Then You will need to set 2 environment variables:

```
TWITTER_API_KEY=xxxxxxxxxxxxxxxxxxxxxxxxx
TWITTER_API_SECRET=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

## Available Commands

when you source the


## TL;DR

Twitter has 2 main authentication method:

- [OAuth signed](https://dev.twitter.com/docs/auth/authorizing-request) issues requests on behalf of a twitter user
- [Application-only](https://dev.twitter.com/docs/auth/application-only-auth) issues requests on behalf of the application itself

The first one is quite complicated as you have to use a lot of http headers:
`oauth_nonce`, `oauth_timestamp` ... and than calculate the `oauth_signature`
using sha1

So this app is using the *Application-only* version
