# Vizio

Basic blocks Vizio viewing-data, ad measurement, diagnostic, and data-streaming endpoints. Strict includes the basic rules and blocks Netflix, firmware updates, and additional TV services. Max includes strict and broadly blocks Vizio and SmartCast services for TVs used mainly as displays.

```text
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/vizio/vizio-basic.txt
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/vizio/vizio-strict.txt
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/vizio/vizio-max.txt
```

## Verification

The device's DNS log includes the ad measurement, data-streaming, firmware update, and TV service domains, two Sentry subdomains, two viewing-data endpoints, and Netflix domains. Blocking behavior has not yet been verified on the device. `users.tvinteractive.tv` has not been observed in the log. The AWS IoT rule is enabled in strict and commented out in basic pending testing.

The Kinesis endpoint is shared by other AWS services, so blocking it can affect other devices.

Max can disrupt Vizio apps, casting, updates, and other smart features. It does not guarantee that the TV is offline. HDMI behavior and blocking effects have not been tested.

Keep basic rules in strict and max, and strict rules in max.
