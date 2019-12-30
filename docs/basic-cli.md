---
title: Basic CLI
nav_order: 2
---

## Cryptogen, Configtxgen, Docker and bash scripts

This demonstrator illustrate the steps involved in using `cryptogen` and `configtxgen` to generate:

* Membership Service Providers (MSP)
* Genesis block
* Channel artefacts

The demonstrator has been verified to work on macOS these versions of Hyperledger Fabric components:

| Component | Version |
| :-- | :-- |
| FABRIC_TOOL | 1.4 |
| macOS | Catalina |
| Docker | version 19.03.4, build 9013bf5 |

## How to use this demonstrator

STEP 1: `git clone https://github.com/fabric-devkit/core-cryptoconfig`.

STEP 2: `cd` into the folder `basic-cli`.

STEP 3: Study the file `crypto-config.yaml`. This contains specifications of the crypto materials for `orderers` and `peers` MSP. Please refer to the [official documentation](https://hyperledger-fabric.readthedocs.io/en/release-1.4/commands/cryptogen.html) for detail explanations behind the configuration file.

STEP 4: Study the file `configtx.yaml`. This contains specifications for genesis blocks and channel configuration. Please refer to the [official documentation](https://hyperledger-fabric.readthedocs.io/en/release-1.4/commands/configtxgen.html) for detail explanations behind the specification.

STEP 5: To see how MSP, genesis block and channel configuration are generated, checkout the bash scripts named `generate-*.sh`. To demonstrate the outcome of using `cryptogen` and `configtxgen`, use the script `./ops.sh` and run the following commands:

* `./ops.sh certs` - to generate MSPs
* `./ops.sh genesis` - to generate genesis block
* `./ops.sh channel` - to generate channel configuration artefacts to be loaded to appropriate orderers.
* `./ops.sh shell` - to give you access to `cryptogen` and `configtxgen` packaged in an official docker image called `hyperledger/fabric-tools`.

## Copyright Notice

Copyright (c) 2019. The Fabric-DevKit Authors. All rights reserved.
SPDX-License-Identifier: Apache-2.0