<div align="center">

# �� Awesome Julia Security

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Julia](https://img.shields.io/badge/Julia-9558B2?style=flat-square&logo=julia&logoColor=white)](https://julialang.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/)

**A curated list of awesome Julia packages, tools, and resources for security research, cryptography, network analysis, and more.**

[Julia](https://julialang.org/) combines Python-like readability with C-like performance, making it ideal for security applications requiring both rapid development and computational efficiency.

</div>

---

## Contents

- [Cryptography](#cryptography)
- [Network Security](#network-security)
- [Forensics](#forensics)
- [Credential Management](#credential-management)
- [Hash Analysis](#hash-analysis)
- [Vulnerability Research](#vulnerability-research)
- [Machine Learning Security](#machine-learning-security)
- [Threat Intelligence](#threat-intelligence)
- [Privacy & Anonymity](#privacy--anonymity)
- [Binary Analysis](#binary-analysis)
- [Web Security](#web-security)
- [Fuzzing](#fuzzing)
- [Security Frameworks](#security-frameworks)
- [Learning Resources](#learning-resources)

---

## Cryptography

*Cryptographic primitives, protocols, and analysis tools.*

### Core Libraries
- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) ⭐50 - Performant, 100% native-Julia SHA-1, SHA-2, and SHA-3 implementation.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) ⭐20 - MD5 hash implementation in pure Julia.
- [Nettle.jl](https://github.com/JuliaCrypto/Nettle.jl) ⭐55 - Julia wrapper for libnettle (MD5, SHA, HMAC, AES).
- [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) ⭐41 - Wrapper around mbedtls for TLS/SSL and crypto.

### Encryption & Ciphers
- [AES.jl](https://github.com/kanav99/AES.jl) ⭐12 - AES encryption On-the-Fly mode implementation.
- [ChaChaCiphers.jl](https://github.com/kernelmethod/ChaChaCiphers.jl) ⭐3 - GPU-compatible ChaCha stream cipher implementations.
- [Sodium.jl](https://github.com/amitmurthy/Sodium.jl) ⭐6 - Julia wrapper for libsodium (NaCl).

### Elliptic Curves & Signatures
- [ECC.jl](https://github.com/roshii/ECC.jl) ⭐6 - Elliptic Curve Cryptography (secp256k1).
- [CryptoSignatures.jl](https://github.com/PeaceFounder/CryptoSignatures.jl) ⭐9 - Cryptographic signature library.
- [CryptoGroups.jl](https://github.com/PeaceFounder/CryptoGroups.jl) ⭐6 - Groups for cryptographic applications.

### Advanced Cryptography
- [ToyFHE.jl](https://github.com/JuliaCrypto/ToyFHE.jl) ⭐95 - Toy implementation of Fully Homomorphic Encryption.
- [NistyPQC.jl](https://github.com/erich-9/NistyPQC.jl) ⭐8 - Post-Quantum Cryptography for Julia.
- [Bcrypt.jl](https://github.com/2HgO/Bcrypt.jl) ⭐2 - bcrypt adaptive hashing algorithm.
- [CryptographicHashFunctions.jl](https://github.com/erich-9/CryptographicHashFunctions.jl) ⭐2 - Fast cryptographic hash functions.

### Utilities
- [CryptoUtils.jl](https://github.com/fcasal/CryptoUtils.jl) ⭐5 - Cryptography and number-theory primitives.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - High-performance security toolkit with SHA3-256, ChaCha20-Poly1305, and entropy analysis.

## Network Security

*Network analysis, port scanning, and protocol tools.*

### Scanning & Reconnaissance
- [**NetProbe**](https://github.com/bad-antics/netprobe) 🆕 - Network reconnaissance and port scanning toolkit with service detection and CIDR support.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - Network forensics with PCAP analysis and protocol dissection.

### Core Networking
- [Sockets.jl](https://github.com/JuliaLang/julia/blob/master/stdlib/Sockets/src/Sockets.jl) - Standard library for network socket programming.
- [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) - HTTP client and server functionality.
- [DNS.jl](https://github.com/JuliaWeb/DNS.jl) - DNS client for Julia.
- [GnuTLS.jl](https://github.com/JuliaWeb/GnuTLS.jl) ⭐8 - Transport Level Security via GnuTLS.

### Protocols
- [LibSSH2.jl](https://github.com/JuliaWeb/LibSSH2.jl) - SSH2 protocol implementation.
- [LibPQ.jl](https://github.com/invenia/LibPQ.jl) - PostgreSQL client library.

## Forensics

*Digital forensics and incident response tools.*

- [FileIO.jl](https://github.com/JuliaIO/FileIO.jl) - Load/save files of various formats.
- [Mmap.jl](https://docs.julialang.org/en/v1/stdlib/Mmap/) - Memory-mapped file access.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - Memory forensics, process analysis, and artifact extraction.

## Credential Management

*Secure credential storage and password utilities.*

- [**SecureVault**](https://github.com/bad-antics/securevault) 🆕 - Encrypted credential vault with PBKDF2 key derivation, secure memory wiping, and audit logging.
- [Bcrypt.jl](https://github.com/2HgO/Bcrypt.jl) ⭐2 - Bcrypt password hashing.

## Hash Analysis

*Hash identification, cracking, and analysis tools.*

- [**HashForensics**](https://github.com/bad-antics/hashforensics) 🆕 - Hash identification, analysis and cracking toolkit with 40+ algorithm support.
- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) ⭐50 - Native SHA implementations for hash generation.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) ⭐20 - MD5 implementation for legacy hash support.

## Vulnerability Research

*Vulnerability discovery and analysis tools.*

- [**Oracle**](https://github.com/bad-antics/oracle) ⭐ - AI-powered vulnerability prediction with 87% accuracy. GNN-based pattern recognition, CVE trend analysis.
- [JuliaLang/SecurityAdvisories.jl](https://github.com/JuliaLang/SecurityAdvisories.jl) ⭐17 - The Julia Security Advisory Database.

## Machine Learning Security

*Adversarial ML, model security, and AI safety tools.*

- [Flux.jl](https://github.com/FluxML/Flux.jl) - Machine learning stack for Julia.
- [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl) - Machine learning framework.
- [Knet.jl](https://github.com/denizyuret/Knet.jl) - Deep learning framework.
- [**Mirage**](https://github.com/bad-antics/mirage) ⭐ - Adversarial ML framework with FGSM, PGD, C&W attacks, model extraction, and robustness testing.
- [**Oracle**](https://github.com/bad-antics/oracle) ⭐ - ML-based vulnerability prediction using graph neural networks.
- [MKTFHE](https://github.com/SNUCP/MKTFHE) ⭐18 - Multi-Key TFHE implementation for secure computation.

## Threat Intelligence

*Threat feeds, IOC management, and intelligence platforms.*

- [**Vortex**](https://github.com/bad-antics/vortex) ⭐ - Threat intelligence fusion platform. 50+ feeds, ML correlation, MITRE ATT&CK mapping, STIX/TAXII support.

## Privacy & Anonymity

*Privacy-preserving technologies and anonymous communication.*

- [**Phantom**](https://github.com/bad-antics/phantom) ⭐ - Zero-knowledge proofs for anonymous vulnerability disclosure. zk-SNARKs implementation.
- [PeaceFounder.jl](https://github.com/PeaceFounder/PeaceFounder.jl) ⭐19 - E2E verifiable evoting via pseudonym braiding.
- [ElectionGuardVerifier.jl](https://github.com/mitre/ElectionGuardVerifier.jl) ⭐8 - MITRE Election Guard verification.

## Binary Analysis

*Binary analysis, reverse engineering, and malware research.*

- [Libdl.jl](https://docs.julialang.org/en/v1/stdlib/Libdl/) - Dynamic linker utilities.
- [DWARF.jl](https://github.com/JuliaDebug/DWARF.jl) - DWARF debug information parser.
- [ELF.jl](https://github.com/JuliaInterop/ELF.jl) - ELF binary format parser.
- [MachO.jl](https://github.com/JuliaInterop/MachO.jl) - Mach-O binary format parser.

## Web Security

*Web application security testing and analysis.*

- [Gumbo.jl](https://github.com/JuliaWeb/Gumbo.jl) - HTML5 parser.
- [Cascadia.jl](https://github.com/Algocircle/Cascadia.jl) - CSS selector implementation.
- [JSON.jl](https://github.com/JuliaIO/JSON.jl) - JSON parsing and generation.
- [URIs.jl](https://github.com/JuliaWeb/URIs.jl) - URI parsing.

## Fuzzing

*Fuzz testing and automated vulnerability discovery.*

- [Fuzz.jl](https://github.com/danluu/Fuzz.jl) - Fuzzing library for Julia.
- [PropCheck.jl](https://github.com/Seelengrab/PropCheck.jl) - Property-based testing.

## Security Frameworks

*Comprehensive security toolkits and frameworks.*

| Package | Description | Lines |
|---------|-------------|-------|
| [**Spectra**](https://github.com/bad-antics/spectra) | High-performance cryptography, network, and forensics toolkit | 8,000+ |
| [**Oracle**](https://github.com/bad-antics/oracle) | AI vulnerability prediction with NVD/MITRE integration | 11,389 |
| [**Phantom**](https://github.com/bad-antics/phantom) | Zero-knowledge proof framework | 6,302 |
| [**Vortex**](https://github.com/bad-antics/vortex) | Threat intelligence platform with ML correlation | 8,406 |
| [**Mirage**](https://github.com/bad-antics/mirage) | Adversarial machine learning framework | 7,000+ |
| [**SecureVault**](https://github.com/bad-antics/securevault) 🆕 | Encrypted credential storage | 700+ |
| [**HashForensics**](https://github.com/bad-antics/hashforensics) 🆕 | Hash identification and cracking | 900+ |
| [**NetProbe**](https://github.com/bad-antics/netprobe) 🆕 | Network reconnaissance toolkit | 900+ |

## Learning Resources

### Tutorials
- [Julia Security Best Practices](https://docs.julialang.org/en/v1/manual/faq/#Security) - Official Julia security FAQ.
- [Cryptography in Julia](https://juliacrypto.github.io/) - JuliaCrypto organization docs.

### Books
- [Julia High Performance](https://www.packtpub.com/product/julia-high-performance-second-edition/9781788298117) - Performance optimization techniques.
- [Hands-On Design Patterns in Julia](https://www.packtpub.com/product/hands-on-design-patterns-and-best-practices-with-julia/9781838648817) - Design patterns for robust Julia code.

### Communities
- [JuliaCrypto](https://github.com/JuliaCrypto) - Cryptography packages organization.
- [Julia Discourse - Security](https://discourse.julialang.org/c/domain/security) - Security discussions.
- [Julia Slack](https://julialang.org/slack/) - #security channel.

---

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [bad-antics](https://github.com/bad-antics) has waived all copyright and related or neighboring rights to this work.

---

<div align="center">

**[⬆ Back to Top](#contents)**

*Part of the [NullSec](https://github.com/bad-antics/nullsec-linux) ecosystem*

</div>
