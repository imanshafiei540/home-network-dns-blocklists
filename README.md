# Home Network DNS Blocklists

DNS blocklists for home devices and services. I'll update the lists as I verify domains on my own devices. Each list notes what has been verified.

## Lists

| List | Blocks |
| --- | --- |
| [Vizio](lists/vizio/) | Basic, strict, and max lists for Vizio devices |

## AdGuard Home

Add the raw list URL under **Filters → DNS blocklists → Add blocklist → Add a custom list**.

```text
https://raw.githubusercontent.com/imanshafiei540/home-network-dns-blocklists/main/lists/vizio/vizio-basic.txt
```

The lists use AdGuard-style rules. Each rule applies to all clients and includes subdomains.

## Pi-hole

Pi-hole supports domain and hosts lists, but wildcard matching differs from AdGuard Home. This list has not been tested with Pi-hole.

