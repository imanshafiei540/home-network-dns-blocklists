# Google TV

Basic blocks ad, analytics, and diagnostic domains. Strict includes basic and also blocks services such as the launcher, Assistant, and connectivity checks.

```text
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/google-tv/google-tv-basic.txt
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/google-tv/google-tv-strict.txt
```

## Verification

The domains or their subdomains were observed in an Onn Google TV box's DNS log. DNS requests don't identify the app or show their contents. Blocking behavior still needs testing on the device; the purpose of the research-related domains in strict needs further verification.

Strict can affect the home screen, voice features, streaming, and other app features. All rules apply to every client using the list; some domains are shared by other devices and apps.

Keep the basic rules in strict when updating them.

## References

- [Perflyst Smart TV list](https://github.com/Perflyst/PiHoleBlocklist/blob/master/SmartTV-AGH.txt) includes the launcher endpoint.
- [AdGuard Tracking Protection filter](https://github.com/AdguardTeam/AdguardFilters/blob/master/SpywareFilter/sections/tracking_servers.txt) includes the Crashlytics reports endpoint.
- [Firebase Android SDK](https://github.com/firebase/firebase-android-sdk/issues/7309) identifies Crashlytics endpoints.
