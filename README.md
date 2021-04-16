# Adax heaters

![Validate with hassfest](https://github.com/Danielhiversen/home_assistant_adax/workflows/Validate%20with%20hassfest/badge.svg)
[![GitHub Release][releases-shield]][releases]
[![hacs_badge][hacs-shield]][hacs]

Custom component for using [Adax](https://adax.no/en/) heaters in Home Assistant.

[Support Daniel Hiversen, the original developer](http://paypal.me/dahoiv)

## Install

Use [hacs](https://hacs.xyz/). To install with HACS add https://github.com/jon-hedgerows/home_assistant_adax as a custom repository, and then install the Adax Heaters Integration.
Or copy the files to the custom_components folder in Home Assistant.

## Configuration (2 options)

You have two alternatives. In either case, you'll need the Account ID (which can be found in the Adax Wifi app, pressing 'Account'). You will also need a credential, which you can create in the 'Account' pane, selecting 'Remote user client API'. A new pane will open and you need to press 'Add credential', after which you should copy the password.

Alternative 1:
Go to integration page in HA, press + and search for Adax
Enter your account id as Account ID
Enter your credential password

Alternative 2:
In configuration.yaml:

```
climate:
  - platform: adax
    account_id: "112395"  # replace with your account ID
    password: "6imtpX63D5WoRyKh"  # replace with your credential password
```

## API

API details: https://adax.no/om-adax/api-development/
