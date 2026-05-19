..
   SPDX-License-Identifier: AGPL-3.0-or-later

   ----------------------------------------------------------------------
   Copyright © 2024, 2025, 2026  Pellegrino Prevete

   All rights reserved
   ----------------------------------------------------------------------

   This program is free software: you can redistribute it and/or modify
   it under the terms of the GNU Affero General Public License as
   published by the Free Software Foundation, either version 3 of the
   License, or (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU Affero General Public License for more details.

   You should have received a copy of the GNU Affero General Public
   License along with this program.
   If not, see <https://www.gnu.org/licenses/>.


=================
erc20-token-send
=================

--------------------------------------------------------------
Ethereum *RC-20 token sender tool
--------------------------------------------------------------
:Version: erc20-token-send |version|
:Manual section: 1


Synopsis
========

erc20-token-send
  *[options]*
  *quiet*
  *retries-max*
  *call-timeout*
  *wallet-seed-path*
  *api-key-path*
  *api-key-path*
  *network*
  *address*
  *abi-path*
  *token-bytecode-path*
  *token-compiler-output-path*
  *receipt-file-path*
  *recipient-address*
  *amount*


Description
===========

Send an amount of \*RC-20 token to an address
on an Ethereum Virtual Machine network.


Networks
=========

All those supported by
'evm-chains-info' as
well as direct RPC addresses.

Arguments
=======

* *quiet*

  Enable verbose output.
  Can be 'y' or 'n'.


* *retries-max*

  Maximum number of retries before failing.


* *call-timeout*

  How many milliseconds to wait for a return
  before declaring the call failed.


* *wallet-seed-path*

  Path of the file containing the seed phrase.


* *api-key-path*

  Path of the API key for the contract ABI
  service provider.


* *network*

  Network on which the contract resides.
  It can be a chain ID or an RPC address.


* *token-address*

  Address of the token contract on the specified
  network.


* *token-abi-path*

  Token ABI file path (JSON).
 

* *token-bytecode-path*

  Path for the token bytecode.


* *token-compiler-output-path*

  Path for the token compiler output path
  (the hardhat artifact).
 

* *measure-unit*

  Measure unit for the transaction value.
  It can be 'wei' or 'ether'.


* *receipt-file-path*

  If specified, will save the transaction
  receipt at the path.


* *amount*

  How much of *measure-unit* of the specified
  token to send to the recipient address.


Application options
=====================

-h                      Display help.


Bugs
====

https://github.com/themartiancompany/erc20-tools/-/issues


Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* evm-contract-deployer-get
* evm-contract-deployment-address
* evm-contract-deployments-dir
* evm-contract-deployment-networks
* evm-contract-deployment-versions
* evm-contracts-abi-get
* evm-wallet

.. include:: variables.rst
