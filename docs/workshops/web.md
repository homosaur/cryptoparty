# Security and Privacy on the Web

## Introduction

The core of almost everyone's Internet usage, no matter what their user profile,
is the web. For most people, increasing their security on the web, is one of the
greatest wins a user can easily accomplish. With even more effort, users can
build an incredibly low risk workspace with little technical expertise.

## TODO: Threat Vectors

*   Mass surveillance (metadata/digital traces)
*   Man in the middle
*   Browser exploits
*   Data leakage (JS, Flash, etc)

## Improving Browsing

### Domain Name System (DNS)

In general your first contact through the outside world from your browser is
not to any particular web server but to the Domain Name System (DNS). You can
pick a public DNS like Google Public or OpenDNS which will help protect against
some censorship and malware, but understand that you should also assume these
services are logging requests. They should probably not be considered
trustworthy.

The best tech you can use right now is [DNSCrypt][1] with a service that
has no logging and transparent governance. The only service I can currently
recommend in that space is [OpenNIC][2], which is compatible with plain old DNS.
You can point to the OpenNIC servers using your DNSCrypt client.

  [1]: https://www.dnscrypt.org
  [2]: https://www.opennicproject.org

### Virtual Private Networks (VPN)

If you ignore the rest of the advice in this document, do not ignore this. The
best way to insure private communications on any network is a VPN. With a VPN,
you are assured a private Internet connection under all circumstances. Even on
unsecured public networks, connections through SSL such as HTTPS websites are
private but standard HTTP connections including many email servers are not. It's
a good baseline for any remote, untrusted connections or if you are attempting
to skirt censorship, surveillance, or geolocation.

You should never use an untrusted or free VPN ever. Assume all free VPNs are
honeypots. It's not possible to run a highly available, high traffic service for
free. Find a service that has a good reputation and does not maintain logs. It
should support L2TP, OpenVPN, SSTP, or another secure protocol. You should never
use PPTP as it is broken security-wise. Get something that works on your mobile
devices also. If you need to purchase anonymously, make sure your service
supports anonymous cryptocurrency such as Bitcoin.

#### VPN Suggestions

*   [Private Internet Access](https://www.privateinternetaccess.com)
*   [NordVPN](https://nordvpn.com)
*   [TorGuard](https://torguard.net)
*   [IPVanish](https://www.ipvanish.com)

### Obtaining or Creating a Better Browser

The core task to tackle when improving your web experience is to upgrade your
primary interface, the browser. You can do this by downloading plugins for your
current browser or by downloading a more secure browser. You may have heard of
the Tor Browser, which solves a slightly different problem than most of what we
discuss here, so we'll cover this in another section.

#### Avoid Flash, Silverlight, etc

## Workshop Resources

*   [DNSCrypt](https://www.dnscrypt.org)
*   [OpenNIC](https://www.opennicproject.org)
