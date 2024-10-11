---
layout: post
toc: true
title: Atumn (Game Content)
---

The atum server provides title content. It always requires an [edge token](/docs/switch/dauth).

* [Overview](#overview)
* [Request headers](#request-headers)

## Overview

The following files are provided by the server:

* `/c1/a/d/<title id>`: control [NCA] for title (icon and name)
* `/c1/a/d/<title id>/<title version>`: control [NCA] for title (icon and name)
* `/c1/t/a/<title id>/<title version>`: [NCA] containing [CNMT]
* `/c1/<title id>/c/a/<content id>`: [NCA] containing [CNMT]
* `/c1/<title id>/c/c/<content id>`: [NCA] containing game content
* `/c1/<title id>/c/c/<content id>/d`: JSON object containing content hashes
* `/c2/<title id>/c/a/<content id>`: [NCA] containing [CNMT]
* `/c2/<title id>/c/c/<content id>`: [NCA] containing game content
* `/c2/<title id>/c/c/<content id>/d`: JSON object containing content hashes

The difference between `c1` and `c2` is that `c1` requires an edge token from [dauth](/docs/switch/dauth), while `c2` requires an edge token from [dragons](/docs/switch/dragons).

## Request Headers

| Header                    | Description                      |
|---------------------------|----------------------------------|
| Host                      | `atum.hac.lp1.d4c.nintendo.net`  |
| Accept                    | `*/*`                            |
| User-Agent                | [User agent](#user-agents)       |
| X-Nintendo-DenebEdgeToken | [Edge token](/docs/switch/dauth) |

For requests ending in `/d`, the `Accept` header contains `application/json` instead and comes after the edge token header.

### User Agents

The user agent looks as follows: `NintendoSDK Firmware/<firmware version>-<revision> (platform:NX; did:<device id>; eid:lp1)`. The firmware version and revision number are obtained from the [system version title](https://switchbrew.org/wiki/System_Version_Title).

Here is an example: `NintendoSDK Firmware/15.0.0-4.0 (platform:NX; did:6265ca40780b1c0d; eid:lp1)`

[CNMT]: https://switchbrew.org/wiki/CNMT
[NCA]: https://switchbrew.org/wiki/NCA
[NCAs]: https://switchbrew.org/wiki/NCA
