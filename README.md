# A Target Privacy Threat Model for the Web

This repository proposes a rough target privacy threat model for the Web.

As a **threat model**, it describes attacker capabilities and attacker goals, and
says which goals which capabilities should and should not enable.

As a **privacy** threat model, the attacker goals compromise the privacy of users,
rather than their security.

As a **target** threat model, it describes not the current state of the Web
including all current maybe-unwise APIs, but rather an end state that we hope to
migrate to, and that new APIs should be held to. This is meant to be a
*plausible* threat model: it doesn't expect to remove any APIs or browser
behavior that is deemed essential to the viability of the Web.

Since people are likely to disagree about which APIs are essential to the Web,
when saying that an attacker can achieve their goal, we describe how the attacker
achieves it using particular "essential" APIs, and we provide an index of those
APIs so people can point out ones that they don't consider essential.
