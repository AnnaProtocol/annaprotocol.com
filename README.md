# ANNΛ Protocol — Official website

This repository hosts the **public-facing website** for ANNA Protocol (Artificial Neural Network for Accountability), including its browser-based attestation verification interface.

**Live site:** https://annaprotocol.com

## Repository contents

| File | Purpose |
| --- | --- |
| `index.html` | Main website |
| `verify.html` | Public attestation lookup and blockchain data display |
| `verifybackup.html` | Historical backup of the verification page |
| `CNAME` | GitHub Pages custom-domain mapping |
| `.htaccess` | Server configuration file; **GitHub Pages does not process Apache .htaccess directives** |

## Verify an attestation

Open https://annaprotocol.com/verify.html and enter an attestation identifier. The verification page queries blockchain contract data through a public RPC endpoint and displays available metadata, hashes, and verification status.

**Important:** The blockchain status is the status reported by the deployed contracts. A verified status is not, by itself, a guarantee of factual correctness of an AI output.

## Related components

- [Dashboard deployment repository](https://github.com/AnnaProtocol/dashboard.annaprotocol.online)
- [Dashboard live application](https://dashboard.annaprotocol.online)
- [Project overview](https://github.com/AnnaProtocol/annaprotocol)
- [Organization](https://github.com/AnnaProtocol)

## Publishing changes

This is a static-site repository. Changes to `index.html` or `verify.html` are committed directly to the source repository and published through its configured GitHub Pages workflow. Check GitHub Pages settings for the deployment branch and folder before changing them.

Do not place private keys, RPC credentials, API tokens, or other secrets in public HTML or JavaScript. Browser code and committed files are publicly accessible.

## Status

Public testnet-facing prototype. Contract addresses and RPC configuration should be checked against the deployed environment before relying on verification results.

**Founder / developer:** Antonio Rufino.
