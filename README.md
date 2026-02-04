<!--
SEO Keywords: Julia security, Julia cryptography, Julia hacking, Julia pentesting,
Julia forensics, Julia network security, Julia adversarial ML, Julia vulnerability research,
Julia blockchain, Julia web3, Julia quantum cryptography, Julia post-quantum,
JuliaCrypto, awesome list, security tools, Julia packages, bad-antics
-->

<div align="center">

```
  █████╗ ██╗    ██╗███████╗███████╗ ██████╗ ███╗   ███╗███████╗          ██╗██╗   ██╗██╗     ██╗ █████╗ 
 ██╔══██╗██║    ██║██╔════╝██╔════╝██╔═══██╗████╗ ████║██╔════╝          ██║██║   ██║██║     ██║██╔══██╗
 ███████║██║ █╗ ██║█████╗  ███████╗██║   ██║██╔████╔██║█████╗            ██║██║   ██║██║     ██║███████║
 ██╔══██║██║███╗██║██╔══╝  ╚════██║██║   ██║██║╚██╔╝██║██╔══╝       ██   ██║██║   ██║██║     ██║██╔══██║
 ██║  ██║╚███╔███╔╝███████╗███████║╚██████╔╝██║ ╚═╝ ██║███████╗     ╚█████╔╝╚██████╔╝███████╗██║██║  ██║
 ╚═╝  ╚═╝ ╚══╝╚══╝ ╚══════╝╚══════╝ ╚═════╝ ╚═╝     ╚═╝╚══════╝      ╚════╝  ╚═════╝ ╚══════╝╚═╝╚═╝  ╚═╝
               ███████╗███████╗ ██████╗██╗   ██╗██████╗ ██╗████████╗██╗   ██╗
               ██╔════╝██╔════╝██╔════╝██║   ██║██╔══██╗██║╚══██╔══╝╚██╗ ██╔╝
               ███████╗█████╗  ██║     ██║   ██║██████╔╝██║   ██║    ╚████╔╝ 
               ╚════██║██╔══╝  ██║     ██║   ██║██╔══██╗██║   ██║     ╚██╔╝  
               ███████║███████╗╚██████╗╚██████╔╝██║  ██║██║   ██║      ██║   
               ╚══════╝╚══════╝ ╚═════╝ ╚═════╝ ╚═╝  ╚═╝╚═╝   ╚═╝      ╚═╝   
                        [ JULIA SECURITY PACKAGES | bad-antics ]
```

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/bad-antics/awesome-julia-security?style=flat-square&logo=github)](https://github.com/bad-antics/awesome-julia-security/stargazers)
[![License: CC0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

**A curated list of Julia packages for security research, cryptography, forensics, adversarial ML, and more.**

*Julia combines Python-like readability with C-like performance — ideal for security tools requiring both rapid development and computational efficiency.*

[Submit Package](https://github.com/bad-antics/awesome-julia-security/issues/new) • [Report Broken Link](https://github.com/bad-antics/awesome-julia-security/issues) • [Contribute](#contributing)

</div>

---

## Contents

- [Cryptography](#cryptography) — Core, encryption, elliptic curves, PQC
- [Quantum Computing](#quantum-computing--cryptography) — Frameworks, post-quantum
- [Network Security](#network-security) — Packets, protocols, TLS
- [Binary Analysis](#binary-analysis) — RE, ELF, DWARF
- [Forensics](#forensics) — Digital forensics, IR
- [Machine Learning Security](#machine-learning-security) — Adversarial ML
- [Blockchain & Web3](#blockchain--web3) — Crypto, smart contracts
- [Web Security](#web-security) — HTTP, HTML parsing
- [Fuzzing](#fuzzing) — Property-based testing
- [Learning Resources](#learning-resources) — Books, docs, communities

---

## Cryptography

### Core Libraries

| Package | Description |
|---------|-------------|
| [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) | 100% native SHA-1, SHA-2, SHA-3 |
| [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) | Pure Julia MD5 |
| [Nettle.jl](https://github.com/JuliaCrypto/Nettle.jl) | libnettle wrapper (AES, HMAC) |
| [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) | TLS/SSL + crypto |

### Encryption

| Package | Description |
|---------|-------------|
| [AES.jl](https://github.com/kanav99/AES.jl) | AES On-the-Fly mode |
| [ChaChaCiphers.jl](https://github.com/kernelmethod/ChaChaCiphers.jl) | GPU-compatible ChaCha |
| [Sodium.jl](https://github.com/amitmurthy/Sodium.jl) | libsodium (NaCl) wrapper |

### Elliptic Curves

| Package | Description |
|---------|-------------|
| [ECC.jl](https://github.com/roshii/ECC.jl) | secp256k1 |
| [CryptoSignatures.jl](https://github.com/PeaceFounder/CryptoSignatures.jl) | Signature schemes |
| [CryptoGroups.jl](https://github.com/PeaceFounder/CryptoGroups.jl) | Crypto groups |

### Advanced / Post-Quantum

| Package | Description |
|---------|-------------|
| [ToyFHE.jl](https://github.com/JuliaCrypto/ToyFHE.jl) | Fully Homomorphic Encryption |
| [NistyPQC.jl](https://github.com/erich-9/NistyPQC.jl) | NIST PQC candidates |
| [Bcrypt.jl](https://github.com/2HgO/Bcrypt.jl) | bcrypt hashing |

---

## Quantum Computing & Cryptography

### Quantum Frameworks

| Package | Description |
|---------|-------------|
| [Yao.jl](https://github.com/QuantumBFS/Yao.jl) | Extensible quantum circuits |
| [QuantumInformation.jl](https://github.com/iitis/QuantumInformation.jl) | QI toolkit |
| [QuantumOptics.jl](https://github.com/qojulia/QuantumOptics.jl) | Quantum system simulation |
| [ITensors.jl](https://github.com/ITensor/ITensors.jl) | Tensor networks |

---

## Network Security

### Packet Analysis

| Package | Description |
|---------|-------------|
| [Pcap.jl](https://github.com/JuliaIO/Pcap.jl) | libpcap bindings |
| [PacketIO.jl](https://github.com/JuliaPackets/PacketIO.jl) | PCAP read/write |

### Protocols

| Package | Description |
|---------|-------------|
| [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) | HTTP client/server |
| [SSH.jl](https://github.com/JuliaCloud/SSH.jl) | SSH protocol |
| [OpenSSL.jl](https://github.com/JuliaWeb/OpenSSL.jl) | OpenSSL bindings |

---

## Binary Analysis

| Package | Description |
|---------|-------------|
| [ReadELF.jl](https://github.com/JuliaIO/ReadELF.jl) | ELF parser |
| [ObjectFile.jl](https://github.com/JuliaIO/ObjectFile.jl) | Object file handling |
| [DWARF.jl](https://github.com/Keno/DWARF.jl) | Debug info parser |
| [LibBFD.jl](https://github.com/Keno/LibBFD.jl) | GNU BFD bindings |

---

## Forensics

| Package | Description |
|---------|-------------|
| [FileIO.jl](https://github.com/JuliaIO/FileIO.jl) | Universal file formats |
| [Images.jl](https://github.com/JuliaImages/Images.jl) | Steganography detection |
| [ZipFile.jl](https://github.com/fhs/ZipFile.jl) | ZIP analysis |

---

## Machine Learning Security

### Adversarial ML

| Package | Description |
|---------|-------------|
| [Flux.jl](https://github.com/FluxML/Flux.jl) | ML framework |
| [Adversarial.jl](https://github.com/jaypmorgan/Adversarial.jl) | Adversarial attacks |
| [Zygote.jl](https://github.com/FluxML/Zygote.jl) | Autodiff for gradients |

### Privacy

| Package | Description |
|---------|-------------|
| [DifferentialPrivacy.jl](https://github.com/OpenMined/DifferentialPrivacy.jl) | DP algorithms |

---

## Blockchain & Web3

| Package | Description |
|---------|-------------|
| [Bitcoin.jl](https://github.com/JuliaCrypto/Bitcoin.jl) | Bitcoin protocol |
| [Ethereum.jl](https://github.com/pszufe/Ethereum.jl) | Ethereum interaction |
| [Secp256k1.jl](https://github.com/JuliaCrypto/Secp256k1.jl) | secp256k1 curves |

---

## Web Security

| Package | Description |
|---------|-------------|
| [Gumbo.jl](https://github.com/JuliaWeb/Gumbo.jl) | HTML5 parsing |
| [URIs.jl](https://github.com/JuliaWeb/URIs.jl) | URI handling |

---

## Fuzzing

| Package | Description |
|---------|-------------|
| [Supposition.jl](https://github.com/Seelengrab/Supposition.jl) | Property-based testing |
| [PropCheck.jl](https://github.com/Seelengrab/PropCheck.jl) | Property testing |

---

## Learning Resources

### Documentation

- [Julia Security Guide](https://docs.julialang.org/en/v1/manual/security/) — Official docs
- [JuliaCrypto](https://github.com/JuliaCrypto) — Crypto organization

### Communities

- [Julia Discourse - Security](https://discourse.julialang.org/c/domain/security)
- [Julia Slack #security](https://julialang.org/slack/)

---

## Related Lists

- [Awesome Security](https://github.com/sbilly/awesome-security)
- [Awesome Cryptography](https://github.com/sobolevn/awesome-cryptography)
- [Awesome Hacking](https://github.com/carpedm20/awesome-hacking)
- [Awesome Rust Security](https://github.com/AwareSet/awesome-rust-security)

---

## Contributing

Found a Julia security package we missed? [Open an issue](https://github.com/bad-antics/awesome-julia-security/issues/new) or submit a PR!

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

<div align="center">

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

**[GitHub](https://github.com/bad-antics)** • **[NullSec](https://github.com/bad-antics/nullsec)**

*Maintained by [bad-antics](https://github.com/bad-antics)*

</div>
