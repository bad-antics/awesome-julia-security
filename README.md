<div align="center">

# 🔐 Awesome Julia Security

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

- [Nettle.jl](https://github.com/JuliaCrypto/Nettle.jl) - Julia wrapper for libnettle cryptographic library.
- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) - Performant, 100% native-Julia SHA-1, SHA-2, and SHA-3 implementation.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) - MD5 hash implementation in pure Julia.
- [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) - Wrapper around mbedtls for cryptographic operations.
- [Crypto.jl](https://github.com/danielsuo/Crypto.jl) - Julia cryptography library.
- [SEAL.jl](https://github.com/JuliaCrypto/SEAL.jl) - Homomorphic encryption using Microsoft SEAL.
- [ECC.jl](https://github.com/JuliaMath/ECC.jl) - Elliptic Curve Cryptography in Julia.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - High-performance security toolkit with SHA3-256, ChaCha20-Poly1305, and entropy analysis. 8,000+ lines.

## Network Security

*Network analysis, packet capture, and protocol tools.*

- [Sockets.jl](https://github.com/JuliaLang/julia/blob/master/stdlib/Sockets/src/Sockets.jl) - Standard library for network socket programming.
- [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) - HTTP client and server functionality.
- [LibPQ.jl](https://github.com/invenia/LibPQ.jl) - PostgreSQL client library.
- [DNS.jl](https://github.com/JuliaWeb/DNS.jl) - DNS client for Julia.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - Network forensics with PCAP analysis and protocol dissection.

## Forensics

*Digital forensics and incident response tools.*

- [FileIO.jl](https://github.com/JuliaIO/FileIO.jl) - Load/save files of various formats.
- [Mmap.jl](https://docs.julialang.org/en/v1/stdlib/Mmap/) - Memory-mapped file access.
- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - Memory forensics, process analysis, and artifact extraction.

## Vulnerability Research

*Vulnerability discovery and analysis tools.*

- [**Oracle**](https://github.com/bad-antics/oracle) ⭐ - AI-powered vulnerability prediction with 87% accuracy. GNN-based pattern recognition, CVE trend analysis. 11,389 lines.

## Machine Learning Security

*Adversarial ML, model security, and AI safety tools.*

- [Flux.jl](https://github.com/FluxML/Flux.jl) - Machine learning stack for Julia.
- [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl) - Machine learning framework.
- [Knet.jl](https://github.com/denizyuret/Knet.jl) - Deep learning framework.
- [**Mirage**](https://github.com/bad-antics/mirage) ⭐ - Adversarial ML framework with FGSM, PGD, C&W attacks, model extraction, and robustness testing. 7,000+ lines.
- [**Oracle**](https://github.com/bad-antics/oracle) ⭐ - ML-based vulnerability prediction using graph neural networks.

## Threat Intelligence

*Threat feeds, IOC management, and intelligence platforms.*

- [**Vortex**](https://github.com/bad-antics/vortex) ⭐ - Threat intelligence fusion platform. 50+ feeds, ML correlation, MITRE ATT&CK mapping, STIX/TAXII support. 8,406 lines.

## Privacy & Anonymity

*Privacy-preserving technologies and anonymous communication.*

- [**Phantom**](https://github.com/bad-antics/phantom) ⭐ - Zero-knowledge proofs for anonymous vulnerability disclosure. zk-SNARKs implementation. 6,302 lines.

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

- [**Spectra**](https://github.com/bad-antics/spectra) ⭐ - High-performance cryptography, network, and forensics toolkit. NullSec ecosystem integration.
- [**Oracle**](https://github.com/bad-antics/oracle) ⭐ - AI vulnerability prediction framework with NVD/MITRE integration.
- [**Phantom**](https://github.com/bad-antics/phantom) ⭐ - Zero-knowledge proof framework for security research.
- [**Vortex**](https://github.com/bad-antics/vortex) ⭐ - Threat intelligence platform with ML correlation.
- [**Mirage**](https://github.com/bad-antics/mirage) ⭐ - Adversarial machine learning framework.

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
