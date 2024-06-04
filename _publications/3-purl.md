---
title: "PURL: Safe and Effective Sanitization of Link Decoration"
classes: wide
---
[33rd USENIX Security Symposium](https://arxiv.org/abs/2308.03417), **(USENIX Security 2024)**

***Shaoor Munir**, Patrick Lee, Umar Iqbal, Zubair Shafiq, Sandra Siby*
# Abstract

While privacy-focused browsers have taken steps to block third-party cookies and browser fingerprinting, novel tracking methods that bypass existing defenses continue to emerge. Since trackers need to exfiltrate information from the client- to server-side through link decoration regardless of the tracking technique they employ, a promising orthogonal approach is to detect and sanitize tracking information in decorated links. We present PURL, a machine-learning approach that leverages a cross-layer graph representation of webpage execution to safely and effectively sanitize link decoration. Our evaluation shows that PURL significantly outperforms existing countermeasures in terms of accuracy and reducing website breakage while being robust to common evasion techniques. We use PURL to perform a measurement study on top-million websites. We find that link decorations are widely abused by well-known advertisers and trackers to exfiltrate user information collected from browser storage, email addresses, and scripts involved in fingerprinting.