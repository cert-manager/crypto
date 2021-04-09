# cert-manager fork of golang/x/crypto

This is a fork of `golang/x/crypto` with added support for fetching [ACME alternative certificate chains](https://tools.ietf.org/html/rfc8555#section-7.4.2) by Maartje Eyskens.

The support for fetching alternative certificate chains allows us to give users an option to [specify a preferred chain](https://cert-manager.io/docs/release-notes/release-notes-1.0/#preferred-chain) to be fetched i.e from Let's Encrypt.

There is an active CL ([#2777294](https://go-review.googlesource.com/c/crypto/+/277294/)) in upstream `golang/x/crypto` that adds support for fetching alternative certificate chains. Once that gets merged, we will be able to start using upstream again.
