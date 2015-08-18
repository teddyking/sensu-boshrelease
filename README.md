# sensu-boshrelease

This BOSH release can be used to deploy [Sensu](https://sensuapp.org/). The current release configures a single-node Sensu server with the following:

* 1 x sensu-server process
* 1 x sensu-api process
* 1 x uchiwa process (that runs both the back-end API and the web UI)

There is an example [bosh-lite](https://github.com/cloudfoundry/bosh-lite) deployment manifest in the examples directory to help you get started.

## Dependencies

Sensu has a dependency on both RabbitMQ and Redis. These aren't included as part of this BOSH release as there are many excellent, open source releases readily available.

If you're just looking to kick the Sensu tyres and don't want to deploy these additional services yourself, you can sign up for free SaaS accounts at:

* [cloudamqp](https://www.cloudamqp.com/) (RabbitMQ)
* [redislabs](https://redislabs.com/) (Redis)

## A note on compilation

The compilation VMs currently need to have Internet access in order to pull down various dependencies.

## Watch this space

This release is in the very early stages of development; lots of features and improvements are on the way.
