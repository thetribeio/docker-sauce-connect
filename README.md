# Sauce connect proxy for Saucelabs

This docker aims to setup the sauce connect proxy of Saucelabs that allows you to run your Selenium tests on the Saucelabs infrastructure for your private/local website/app.

## Use with `docker`

    docker run thetribe/sauce-connect:4.6.2 sc -v -u SAUCELABS-USER -k SAUCELABS-TOKEN --readyfile sauce-ready

## Use with `docker-compose`

In your `docker-compose.yml`:

    services:
        sauce-connect:
            image: thetribe/sauce-connect:4.6.2
            command: sc -v -u SAUCELABS-USER -k SAUCELABS-TOKEN --readyfile sauce-ready
