# Overview

The purpose of this subproject is to demonstrate the step involve generating [Membership Service Provider (MSP)](https://hyperledger-fabric.readthedocs.io/en/release-1.4/msp.html), genesis blocks and channel configuration (i.e. core crypto materials) 

The principal or baseline tools involved in generating these artefacts are [cryptogen](https://hyperledger-fabric.readthedocs.io/en/release-1.4/commands/cryptogen.html) and [configtxgen](https://hyperledger-fabric.readthedocs.io/en/release-1.4/commands/configtxgen.html).

## Content

| Demonstrator | Description |
| --- | --- |
| `basic-cli` |  This uses a combination of `cryptogen tools`, `configtxgen tools`, `docker` and `bash scripts` to generate core crypto artefacts. |

## Copyright Notice

Copyright (c) 2019. The Fabric-DevKit Authors. All rights reserved.
SPDX-License-Identifier: Apache-2.0
