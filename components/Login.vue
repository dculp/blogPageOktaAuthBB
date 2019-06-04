<template>
  <div class="login">
    <div id="okta-signin-container"></div>
  </div>
</template>

<script>
import OktaSignIn from '@okta/okta-signin-widget'
import '@okta/okta-signin-widget/dist/css/okta-sign-in.min.css'
import '@okta/okta-signin-widget/dist/css/okta-theme.css'
import authConfig from '../.config.js'


export default {
  name: 'Login',
  mounted: function () {
    this.$nextTick(function () {
      this.widget = new OktaSignIn({
        baseUrl: authConfig.oidc.issuer.split('/oauth2')[0],
        clientId: authConfig.oidc.client_id,
        redirectUri: authConfig.oidc.redirect_uri,
        authParams: {
          responseType: ['id_token', 'token'],
          issuer: authConfig.oidc.issuer,
          scopes: authConfig.oidc.scope.split(' '),
          display: 'page'
        }
      })

      this.widget.renderEl(
        { el: '#okta-signin-container' },
        () => {

        },
        (err) => {
          throw err
        }
      )
    })
  },
  destroyed () {
    // Remove the widget from the DOM on path change
    this.widget.remove()
  }
}
</script>

<!-- <script>
  var config = {
    url: 'https://beachbodyciam.oktapreview.com',
    issuer: 'https://beachbodyciam.oktapreview.com/oauth2/default',
    clientId: '0oal7qfzxpANpMYQU0h7',
    redirectUri: 'http://localhost:8080/implicit/callback',
    tokenManager: {
      storage: 'sessionStorage'
    },
  };

  var OktaAuth = require('@okta/okta-auth-js');
  var authClient = new OktaAuth(config);

  authClient.session.get().then(function(session) {
    console.log("Got session:");
    console.log(session);

  authClient.token.getWithoutPrompt({
    responseType: ["id_token", "token"],
    scopes: ["openid", "email"] // or array of types// optional if the user has an existing Okta session
  }).then(function(tokens) {
    console.log("Got tokens:");
    console.log(tokens);
    tokens.forEach(function(token) {
      ['idToken', 'accessToken'].forEach(function(kind) {
        if (kind in token) {
          console.log("Received an " + kind + " from Okta:");
          console.log(token);
          authClient.tokenManager.add(kind, token);
        }
      });
    });
    // [jpf] FIXME: Is this needed?
    var accessToken = authClient.tokenManager.get('accessToken');
    var base64Url = accessToken.accessToken.split('.')[1];
    var base64 = base64Url.replace('-', '+').replace('_', '/');
    var info = JSON.parse(window.atob(base64));
    console.log(info)
  }).else(function() {
    console.log("Didn't get tokens");
  })
})

</script>  -->