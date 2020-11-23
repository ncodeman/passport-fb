# Passport-FB is updated lib with pasReqToCallback

## Installation

    $ npm install passport-fb

## Usage

#### Configure Strategy

Everything is the same as in passport-vkontakte, but allowed passReqToCallback

```javascript
passport.use(new VKontakteStrategy(
  {
    clientID:     FACEBOOK_APP_ID,
    clientSecret: FACEBOOK_APP_SECRET,
    callbackURL:  "http://localhost:3000/auth/facebook/callback",
    passReqToCallback: true // is optional, by default false
  },
  function myVerifyCallbackFn(req, accessToken, refreshToken, profile, done) {
  // Here you can use your request
  }
));
```
