# Awesome Freedom
In this repository we have collected all awesome tools for iranian people.

If you know more tools, please add it in issues or add a pull requests

# Table of Content
- [Telegram Proxy](#telegram-proxy)
- [AntiFilter](#anti-filter)
  - [Server](#server)
    - [Gost](#gost)
    - [Shadowsocks](#shadowsocks)
    - [Outline](#outline)
    - [SoftEther](#softether)
  - [Client](#client)
    - [Clash](#clash)
    - [ServerLess](#serverless)
    - [Shadowsocks](#shadowsocks-client)
    - [Outline](#outline-client)
    - [OpenVpn](#openvpn-client)
    - [Cisco AnyConnect](#cisco-anyconnect-client)
    - [SoftEther Client](#softether-client)
    - [SSTP Client](#sstp-client)
- [List of VPS Provider](vps-providers.md)
- [Free AntiFilter](#free-antifilter)
- [Free AntiFilter with user registration](#free-antiFilter-with-user-registration)

# Telegram Proxy
 **[`^        back to top        ^`](#table-of-content)**
 - [Official Python](https://github.com/alexbers/mtprotoproxy) Easy to setup
 - [Official Python Docker](https://hub.docker.com/r/alexbers/mtprotoproxy) Easy to setup
 - [Official C++](https://github.com/TelegramMessenger/MTProxy) Hard to setup
 
# Anti-Filter
## Server
**[`^        back to top        ^`](#table-of-content)**
### One Click Setup MultiProxy
- [Hiddify](https://hiddify.github.io/setup-proxy-one-click.html)
### Gost
- [Gost](https://github.com/ginuerzh/gost) - Easy to setup but powerful and support nearly all proxy protocol such as tls tunnel ssh golang udp http2 socks5 shadowsocks kcp quic tuntap sni obfs4 dns 
- [Document](https://v2.gost.run/en/)
- [Example Configuration Script](https://github.com/hiddify/config/blob/main/gost/setup_gost.sh)
- Compatible Clients `clash` `outline`
### Shadowsocks
- [Download](https://shadowsocks.org/en/index.html) - A secure proxy, designed to protect your Internet traffic.
- [Tutorial](https://github.com/WeAreMahsaAmini/FreeInternet)
- Compatible Clients `clash` `outline`
### Outline
- [Download](https://getoutline.org/fa/get-started/#step-1) - A secure socks5 proxy, designed to protect your Internet traffic. 
- Compatible Clients `clash` `outline`
### Softether
- [Download](https://www.softether-download.com/en.aspx?product=softether) 
- A simple vpn manager that supports many vpn protocol
- Compatible Clients `pptp` `sstp` `l2tp` `openvpn` `softether`


## Client
**[`^        back to top        ^`](#table-of-content)**
### Clash 
`recommended`
 A Rule Based proxy (based on GEOIP, IP-CIDR, Domain, fallback, load balance) that support many protocols such as Shadowsocks(R), VMess, Trojan, Snell, SOCKS5, HTTP(S) that can be retrive by a link
 #### Clash Download
- [Android: Google Play](https://play.google.com/store/apps/details?id=com.github.kr328.clash) [Android: APK](https://github.com/Kr328/ClashForAndroid/releases/download/v2.5.11/cfa-2.5.11-premium-universal-release.apk) [Android: Repository](https://github.com/Kr328/ClashForAndroid)
- [Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.20.4/Clash.for.Windows.Setup.0.20.4.exe)
- [macOS](https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.20.4/Clash.for.Windows-0.20.4.dmg) 
- [Linux](https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.20.5/Clash.for.Windows-0.20.5-x64-linux.tar.gz)
- [iOS: Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118?platform=iphone) is not free. [How to bypass payment](https://github.com/WeAreMahsaAmini/FreeInternet/blob/main/README.md#ios)  

<!--- [iOS: Stash not free](https://apps.apple.com/app/stash/id1596063349?platform=iphone) not free-->
 
 #### Clash example configuration for Iran
 - [Full tutorial](https://lancellc.gitbook.io/clash)
 - [only pass filtered sites to proxy](https://github.com/hiddify/config/blob/main/clash/lite.yml)  
 It is useful when you want to use always the proxy without having any issues to all other sites. `Fastest solution` `lowest overhead on server`
 - [only pass non-iranian sites to proxy](https://github.com/hiddify/config/blob/main/clash/normal.yml)
 It uses direct connection for irannian sites (50% off in price) and  the non-iranian sites will pass to the proxy so you can avoid external sanctions.
 - [pass all sites to proxy](https://github.com/hiddify/config/blob/main/clash/all.yml) 
 - [Full Clash Configuration](https://github.com/Dreamacro/clash/wiki/Configuration)

### ServerLess!!! 
This approach works by changing packets to scape filtering! 
- requirment: a working DNS over HTTPS (DoH) is needed. [setup a DoH server]()
- [Android](https://github.com/zhenyolka/DPITunnel-android)
- [Windows: GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI) [Windows: GreenTunnel](https://github.com/SadeghHayeri/GreenTunnel)

### Shadowsocks Client
 **we suggest to use clash client instead of shadowsocks client**
- [iOS: OneClick](https://apps.apple.com/us/app/id1545555197) Free, 
[iOS: Potatso](https://apps.apple.com/app/potatso-lite/id1239860606), [iOS: Shadowlink](https://apps.apple.com/us/app/shadowlink-shadowsocks-vpn/id1439686518),  [iOS: Surge 5](https://apps.apple.com/us/app/id1442620678), [iOS: Spectre](https://apps.apple.com/us/app/spectre-vpn/id1508712998) [iOS: oneclick](https://apps.apple.com/us/app/oneclick-safe-easy-fast/id1545555197) Free.
- [iOS: Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118) is not free. [How to bypass payment](https://github.com/WeAreMahsaAmini/FreeInternet/blob/main/guides/shadowsocks-v2ray-tls/how-to-connect.md#%D8%A2%DB%8C%D9%81%D9%88%D9%86-%D9%88-%D8%A2%DB%8C%D9%BE%D8%AF)
- [Android: sagernet](https://play.google.com/store/apps/details?id=io.nekohasekai.sagernet&hl=en&gl=US)
- [Windows](https://github.com/shadowsocks/shadowsocks-windows/releases)
- [macOS](https://github.com/shadowsocks/shadowsocks-windows/releases)

### Outline Client
- [Outline](https://getoutline.org/fa/get-started/#step-3)

### OpenVpn Client
- [Windows](https://openvpn.net/community-downloads/)
- [Android](https://play.google.com/store/apps/details?id=de.blinkt.openvpn)
- [iOS](https://apps.apple.com/fr/app/openvpn-connect/id590379981)
- [macOS](https://openvpn.net/client-connect-vpn-for-mac-os/)
- [Linux](https://openvpn.net/cloud-docs/openvpn-3-client-for-linux/)

### Cisco AnyConnect Client
- [Windows / macOS / linux](https://software.cisco.com/download/home/286281283/type/282364313/release/4.10.05111)
- [Android](https://play.google.com/store/apps/details?id=com.cisco.anyconnect.vpn.android.avf&hl=en&gl=US)
- [iOS](https://apps.apple.com/us/app/cisco-secure-client/id1135064690?platform=iphone)

### Softether Client
- [SoftEther](https://www.softether-download.com/en.aspx?product=softether) 
- A simple vpn client for softether server
### SSTP Client
- Windows -> Built-in
- [Android](https://play.google.com/store/apps/details?id=kittoku.osc&hl=en&gl=US), [Android: apk](https://github.com/kittoku/Open-SSTP-Client/releases/download/v1.5.5/osc-1.5.5.apk)
- [macOS: isstp](https://github.com/axot/isstp), [macOS: sstp-client](https://gitlab.com/eivnaes/sstp-client)
- [Linux](https://gitlab.com/eivnaes/sstp-client)
- [iOS: AnyConnect](https://apps.apple.com/us/app/cisco-anyconnect/id1135064690) not sure works


# Public Free AntiFilter
**[`^        back to top        ^`](#table-of-content)**
- [Tor Project](https://snowflake.torproject.org/)
- [Psiphon: Android](https://play.google.com/store/apps/details?id=com.psiphon3.subscription), [Psiphon: Android Apk](https://psiphon.ca/PsiphonAndroid.apk) [Psiphon: Windows](https://psiphon.ca/psiphon3.exe), [Psiphon: iOS](https://apps.apple.com/app/psiphon/id1276263909), [Psiphon: macOS](https://apps.apple.com/app/psiphon/id1276263909), [Psiphon: By Email](mailto:get@psiphon3.com)
- [Ultrasurf: iOS](https://apps.apple.com/us/app/ultrasurf-vpn/id1563051300), [Ultrasurf: Android](https://play.google.com/store/apps/details?id=us.ultrasurf.mobile.ultrasurf&hl=en_US&gl=US), [Ultrasurf: Windows](https://ultrasurf.us/download/usf.zip), [Ultrasurf: chrome/edge browser](https://chrome.google.com/webstore/detail/ultrasurf-security-privac/mjnbclmflcpookeapghfhapeffmpodij)

# Free AntiFilter with user registration
**[`^        back to top        ^`](#table-of-content)**
- [VpnGate](https://www.vpngate.net/en/)
- [WindScribe](https://windscribe.com) - Free 10 GB VPN

# [List of VPS Providers](vps-providers.md)

# Free Domain Names
- [sslip](https://sslip.io/) and [nip](https://nip.io)
- [many subdomain, us.to, mds.ir, ~40.000 domains](https://freedns.afraid.org/): it is very nice just you need to register an account and point the ip of your-server to a name.
- [.ml, .tk, .ga, .cf, .gq,](https://freenom.com) : Top-level DNS record
- [.free](https://nic.free): Top-level DNS record
- [subdomain, .ze.cx, .fr.nf .biz.st](https://www.nom.za/)
- [subdomain, .1s.fr .be.ma .c0m.at .c4.fr .ch.ma .fr.ht .fr.mu .ht.cx .qc.cx .vu.cx .xl.cx .ze.tc](https://www.venez.fr/)
- [.ipq.co, fdns.uk](https://www.ipq.co/)

- [$1 Domain](https://www.namecheap.com/promos/99-cent-domain-names/)
- [.42.pl](freedns.42.pl)  can create a dns by IP
- [noip](https://www.noip.com/)
