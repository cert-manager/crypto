# cert-manager fork of golang/x/crypto

This is a fork of `golang/x/crypto` with added support for fetching [ACME alternative certificate chains](https://tools.ietf.org/html/rfc8555#section-7.4.2) by Maartje Eyskens.

This was historically used by cert-manager to allow our users to [specify a preferred chain](https://cert-manager.io/docs/release-notes/release-notes-1.0/#preferred-chain) to be fetched i.e from Let's Encrypt.

Since cert-manager v1.4 this fork is no longer used as support for fetching alternate chains was added in upstream go/crypto (CL ([#2777294](https://go-review.googlesource.com/c/crypto/+/277294/)).

This repo remains here so as to not break anyone importing older versions of cert-manager
