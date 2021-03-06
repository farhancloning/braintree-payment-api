# Spring Payment GateWay API using Braintree SandBox.

Braintree integration for SpringBoot (Java).

## Setup Instructions

1. [Install gradle](https://docs.gradle.org/current/userguide/installation.html) and project dependencies:

  ```
  ./gradlew build -x test
  ```

2. Copy the contents of `example.config.properties` into a new file named `config.properties` and fill in your Braintree API credentials. Credentials can be found by navigating to  Account > My User > View Authorizations in the Braintree Control Panel. Full instructions can be [found on our support site](https://articles.braintreepayments.com/control-panel/important-gateway-credentials#api-credentials).

3. Start server:

  ```
  java -jar build/libs/bt-example-0.1.0.jar
  ```

  This starts the server on port `8080` listening to all interfaces.

## Deploying to Heroku

You can deploy this app directly to Heroku to see the app live. Skip the setup instructions above and click the button below. This will walk you through getting this app up and running on Heroku in minutes.

<p><a href="https://heroku.com/deploy?template=https://github.com/farhancloning/BrainTreeCardPaymentAPI&amp;env%5BBT_ENVIRONMENT%5D=sandbox" rel="nofollow"><img src="https://camo.githubusercontent.com/83b0e95b38892b49184e07ad572c94c8038323fb/68747470733a2f2f7777772e6865726f6b7563646e2e636f6d2f6465706c6f792f627574746f6e2e737667" alt="Deploy" data-canonical-src="https://www.herokucdn.com/deploy/button.svg" style="max-width:100%;"></a></p>


## Running tests

All tests are integration tests. Integration tests make API calls to Braintree and require that you set up your Braintree credentials. You can run this project's integration tests by adding your sandbox API credentials to `config.properties` and running `./gradlew test`.


## Pro Tips

* Run `java -Dserver.port=4000 -jar build/libs/bt-example-0.1.0.jar` to start the server on port 4000. Replace `4000` with any number to start it on a different port.


