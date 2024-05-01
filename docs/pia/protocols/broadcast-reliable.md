---
layout: post
toc: true
title: Broadcast Reliable
---

This protocol may be used by games to send data packets to other consoles. The broadcast reliable protocol is similar to the [reliable protocol](/docs/pia/protocols/reliable) in that it uses a [reliable sliding window](/docs/pia/reliable-sliding-window) to ensure that all packets arrive in the correct order. The difference is that the broadcast reliable protocol is able to send broadcast packets in LAN and LDN mode, which makes it more efficient for packets that are sent to all stations in the mesh.
