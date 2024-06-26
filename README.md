<div align="center">
  <img src="docs/logos/logo.jpg" alt="rosettanet" height="400"/>

  **Ethereum <> Starknet RPC middleware.**

  [![Exploration_Team](https://img.shields.io/badge/Exploration_Team-29296E.svg?&style=for-the-badge&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIGlkPSJhIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxODEgMTgxIj48ZGVmcz48c3R5bGU+LmJ7ZmlsbDojZmZmO308L3N0eWxlPjwvZGVmcz48cGF0aCBjbGFzcz0iYiIgZD0iTTE3Ni43Niw4OC4xOGwtMzYtMzcuNDNjLTEuMzMtMS40OC0zLjQxLTIuMDQtNS4zMS0xLjQybC0xMC42MiwyLjk4LTEyLjk1LDMuNjNoLjc4YzUuMTQtNC41Nyw5LjktOS41NSwxNC4yNS0xNC44OSwxLjY4LTEuNjgsMS44MS0yLjcyLDAtNC4yN0w5Mi40NSwuNzZxLTEuOTQtMS4wNC00LjAxLC4xM2MtMTIuMDQsMTIuNDMtMjMuODMsMjQuNzQtMzYsMzcuNjktMS4yLDEuNDUtMS41LDMuNDQtLjc4LDUuMThsNC4yNywxNi41OGMwLDIuNzIsMS40Miw1LjU3LDIuMDcsOC4yOS00LjczLTUuNjEtOS43NC0xMC45Ny0xNS4wMi0xNi4wNi0xLjY4LTEuODEtMi41OS0xLjgxLTQuNCwwTDQuMzksODguMDVjLTEuNjgsMi4zMy0xLjgxLDIuMzMsMCw0LjUzbDM1Ljg3LDM3LjNjMS4zNiwxLjUzLDMuNSwyLjEsNS40NCwxLjQybDExLjQtMy4xMSwxMi45NS0zLjYzdi45MWMtNS4yOSw0LjE3LTEwLjIyLDguNzYtMTQuNzYsMTMuNzNxLTMuNjMsMi45OC0uNzgsNS4zMWwzMy40MSwzNC44NGMyLjIsMi4yLDIuOTgsMi4yLDUuMTgsMGwzNS40OC0zNy4xN2MxLjU5LTEuMzgsMi4xNi0zLjYsMS40Mi01LjU3LTEuNjgtNi4wOS0zLjI0LTEyLjMtNC43OS0xOC4zOS0uNzQtMi4yNy0xLjIyLTQuNjItMS40Mi02Ljk5LDQuMyw1LjkzLDkuMDcsMTEuNTIsMTQuMjUsMTYuNzEsMS42OCwxLjY4LDIuNzIsMS42OCw0LjQsMGwzNC4zMi0zNS43NHExLjU1LTEuODEsMC00LjAxWm0tNzIuMjYsMTUuMTVjLTMuMTEtLjc4LTYuMDktMS41NS05LjE5LTIuNTktMS43OC0uMzQtMy42MSwuMy00Ljc5LDEuNjhsLTEyLjk1LDEzLjg2Yy0uNzYsLjg1LTEuNDUsMS43Ni0yLjA3LDIuNzJoLS42NWMxLjMtNS4zMSwyLjcyLTEwLjYyLDQuMDEtMTUuOGwxLjY4LTYuNzNjLjg0LTIuMTgsLjE1LTQuNjUtMS42OC02LjA5bC0xMi45NS0xNC4xMmMtLjY0LS40NS0xLjE0LTEuMDgtMS40Mi0xLjgxbDE5LjA0LDUuMTgsMi41OSwuNzhjMi4wNCwuNzYsNC4zMywuMTQsNS43LTEuNTVsMTIuOTUtMTQuMzhzLjc4LTEuMDQsMS42OC0xLjE3Yy0xLjgxLDYuNi0yLjk4LDE0LjEyLTUuNDQsMjAuNDYtMS4wOCwyLjk2LS4wOCw2LjI4LDIuNDYsOC4xNiw0LjI3LDQuMTQsOC4yOSw4LjU1LDEyLjk1LDEyLjk1LDAsMCwxLjMsLjkxLDEuNDIsMi4wN2wtMTMuMzQtMy42M1oiLz48L3N2Zz4=)](https://github.com/keep-starknet-strange)

</div>

## Overview

Rosetta is a middleware software that acts like an Ethereum RPC. It makes requests to the Starknet network while outputting Ethereum RPC outputs. This allows users to interact with Starknet the same as they interact with the EVM-compatible chain. 

**Rosetta**
- Rosetta is not a Starknet node itself.
- Rosetta needs a working Starknet node to be connected.
- Rosetta can handle both Starknet and Ethereum RPC requests.

**What does Rosetta benefit to users?**
- [x] You can connect and interact protocols in Starknet with your existing EVM wallet (Metamask, Trust wallet, Hardware wallets, etc.)
- [x] You can use Rosetta on local. There is no sync needed. Simply, users can clone the repo and use their local Rosetta node to connect to Starknet.
- [x] You can use L1 interactive protocols by just changing the network on your wallet.

**What does Rosetta benefit to devs?**
- [x] You can use all EVM-compatible libraries. (Ethers, web3js, etc.)
- [x] If you want to migrate your project from the EVM chain to Starknet, all you need to do is develop your smart contracts with cairo. You just need to care about providing the same ABI in both. You don't need to make any changes on frontend, or backend. Rosetta handles all of these.

**Rosetta aims to give EVM experience to users where they won't ever notify they are using Starknet.**

## Project structure

**Rosettanet:** Middleware software, core part of Rosetta. It acts like a gateway between Starknet and the user. It formats Ethereum RPC requests to the format that Starknet RPC accepts, and formats Starknet RPC responses into Ethereum RPC response. Written in Typescript. In future it also will be developed with Rust.

**Rosetta Accounts:** Account smart contract library will be written in Cairo. Custom account contracts that are able to verify Ethereum account signatures on Starknet to execute and verify transactions.

**Rosetta Verifier:** Starknet smart contracts that verify signatures with format EIP-1559. Converts EVM calldatas into Starknet calldata. This is the core part to achieve non-trusted setup.

**Lens:** Permissionless Starknet smart contract that matches Ethereum addresses with Starknet addresses.

*Additional extensions will be developed to provide integrability for existing Starknet protocols.*

### Contracts

The contracts are located in the `contracts/` directory. It's a `scarb` project, so you can use the `scarb` CLI to build it.

It uses `Starknet Foundry` for tests.

See the [contracts README](contracts/README.md) for more information.

### RPC Server

See the [RPC README](src/README.md) for more information.

## Architecture

Here is a high-level overview of the architecture of Rosettanet:

[![Architecture](docs/architecture.png)](docs/architecture.png)

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ametel01"><img src="https://avatars.githubusercontent.com/u/91626827?v=4?s=100" width="100px;" alt="Alex Metelli"/><br /><sub><b>Alex Metelli</b></sub></a><br /><a href="#code-ametel01" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ermvrs"><img src="https://avatars.githubusercontent.com/u/3417324?v=4?s=100" width="100px;" alt="Erim"/><br /><sub><b>Erim</b></sub></a><br /><a href="#code-ermvrs" title="Code">💻</a> <a href="#test-ermvrs" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Boreas09"><img src="https://avatars.githubusercontent.com/u/90131638?v=4?s=100" width="100px;" alt="Bora Atik"/><br /><sub><b>Bora Atik</b></sub></a><br /><a href="#code-Boreas09" title="Code">💻</a> <a href="#test-Boreas09" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ktarun1419"><img src="https://avatars.githubusercontent.com/u/86646398?v=4?s=100" width="100px;" alt="tarun kaushik"/><br /><sub><b>tarun kaushik</b></sub></a><br /><a href="#code-ktarun1419" title="Code">💻</a> <a href="#test-ktarun1419" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/TropicalDog17"><img src="https://avatars.githubusercontent.com/u/79791913?v=4?s=100" width="100px;" alt="Tuan Tran"/><br /><sub><b>Tuan Tran</b></sub></a><br /><a href="#code-TropicalDog17" title="Code">💻</a> <a href="#test-TropicalDog17" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JimmyFate"><img src="https://avatars.githubusercontent.com/u/158521482?v=4?s=100" width="100px;" alt="Jimmy Fate"/><br /><sub><b>Jimmy Fate</b></sub></a><br /><a href="#code-JimmyFate" title="Code">💻</a> <a href="#test-JimmyFate" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Akashneelesh"><img src="https://avatars.githubusercontent.com/u/66639153?v=4?s=100" width="100px;" alt="Akashneelesh"/><br /><sub><b>Akashneelesh</b></sub></a><br /><a href="#code-Akashneelesh" title="Code">💻</a> <a href="#test-Akashneelesh" title="Tests">⚠️</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://medium.com/@aryangodara_19887"><img src="https://avatars.githubusercontent.com/u/65490434?v=4?s=100" width="100px;" alt="Aryan Godara"/><br /><sub><b>Aryan Godara</b></sub></a><br /><a href="#code-AryanGodara" title="Code">💻</a> <a href="#test-AryanGodara" title="Tests">⚠️</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
