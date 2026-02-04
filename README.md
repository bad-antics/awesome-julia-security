# Awesome Julia Security

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome Julia packages, tools, and resources for security research, cryptography, network analysis, and more.

[Julia](https://julialang.org/) combines Python-like readability with C-like performance, making it ideal for security applications requiring both rapid development and computational efficiency.

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

## Cryptography

Cryptographic primitives, protocols, and analysis tools.

### Core Libraries

- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) - Performant, 100% native-Julia SHA-1, SHA-2, and SHA-3 implementation.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) - MD5 hash implementation in pure Julia.
- [Nettle.jl](https://github.com/JuliaCrypto/Nettle.jl) - Julia wrapper for libnettle (MD5, SHA, HMAC, AES).
- [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) - Wrapper around mbedtls for TLS/SSL and crypto.

### Encryption & Ciphers

- [AES.jl](https://github.com/kanav99/AES.jl) - AES encryption On-the-Fly mode implementation.
- [ChaChaCiphers.jl](https://github.com/kernelmethod/ChaChaCiphers.jl) - GPU-compatible ChaCha stream cipher implementations.
- [Sodium.jl](https://github.com/amitmurthy/Sodium.jl) - Julia wrapper for libsodium (NaCl).

### Elliptic Curves & Signatures

- [ECC.jl](https://github.com/roshii/ECC.jl) - Elliptic Curve Cryptography (secp256k1).
- [CryptoSignatures.jl](https://github.com/PeaceFounder/CryptoSignatures.jl) - Cryptographic signature library.
- [CryptoGroups.jl](https://github.com/PeaceFounder/CryptoGroups.jl) - Groups for cryptographic applications.

### Advanced Cryptography

- [ToyFHE.jl](https://github.com/JuliaCrypto/ToyFHE.jl) - Toy implementation of Fully Homomorphic Encryption.
- [NistyPQC.jl](https://github.com/erich-9/NistyPQC.jl) - Post-Quantum Cryptography for Julia.
- [Bcrypt.jl](https://github.com/2HgO/Bcrypt.jl) - bcrypt adaptive hashing algorithm.

## Network Security

Network analysis, protocol implementation, and security monitoring.

### Packet Analysis

- [Pcap.jl](https://github.com/JuliaIO/Pcap.jl) - libpcap bindings for packet capture.
- [PacketIO.jl](https://github.com/JuliaPackets/PacketIO.jl) - Read and write network packet captures.

### Protocol Implementation

- [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) - HTTP client/server implementation with security features.
- [SSH.jl](https://github.com/JuliaCloud/SSH.jl) - SSH protocol implementation.
- [Sockets.jl](https://docs.julialang.org/en/v1/stdlib/Sockets/) - Low-level socket programming (stdlib).

### TLS/SSL

- [OpenSSL.jl](https://github.com/JuliaWeb/OpenSSL.jl) - OpenSSL bindings for Julia.
- [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) - TLS/SSL implementation.

## Forensics

Digital forensics and incident response tools.

- [FileIO.jl](https://github.com/JuliaIO/FileIO.jl) - Universal file format support for forensic analysis.
- [Images.jl](https://github.com/JuliaImages/Images.jl) - Image processing for steganography detection.
- [ZipFile.jl](https://github.com/fhs/ZipFile.jl) - ZIP archive analysis.

## Credential Management

Password handling and secure credential storage.

- [Keychain.jl](https://github.com/JuliaSecurity/Keychain.jl) - System keychain access for secure credential storage.
- [Bcrypt.jl](https://github.com/2HgO/Bcrypt.jl) - bcrypt password hashing.

## Hash Analysis

Hash computation and analysis tools.

- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) - SHA family hash functions.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) - MD5 hash implementation.
- [CRC32.jl](https://github.com/JuliaIO/CRC32.jl) - CRC32 checksum computation.

## Vulnerability Research

Tools for vulnerability discovery and analysis.

- [Revise.jl](https://github.com/timholy/Revise.jl) - Live code reloading for rapid exploit development.
- [Debugger.jl](https://github.com/JuliaDebug/Debugger.jl) - Interactive debugging for vulnerability analysis.
- [BenchmarkTools.jl](https://github.com/JuliaCI/BenchmarkTools.jl) - Timing analysis for side-channel research.

## Machine Learning Security

ML/AI security, adversarial attacks, and model robustness.

- [Flux.jl](https://github.com/FluxML/Flux.jl) - ML framework for adversarial ML research.
- [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl) - Machine learning framework.
- [Zygote.jl](https://github.com/FluxML/Zygote.jl) - Automatic differentiation for gradient-based attacks.

## Threat Intelligence

Threat feeds, IOC handling, and intelligence analysis.

- [CSV.jl](https://github.com/JuliaData/CSV.jl) - Fast CSV parsing for threat feeds.
- [JSON3.jl](https://github.com/quinnj/JSON3.jl) - JSON parsing for STIX/TAXII data.
- [DataFrames.jl](https://github.com/JuliaData/DataFrames.jl) - Data analysis for threat intelligence.

## Privacy & Anonymity

Privacy-preserving computation and anonymity tools.

- [ToyFHE.jl](https://github.com/JuliaCrypto/ToyFHE.jl) - Homomorphic encryption for privacy-preserving computation.
- [DifferentialPrivacy.jl](https://github.com/JuliaDiffEq/DifferentialPrivacy.jl) - Differential privacy mechanisms.

## Binary Analysis

Binary parsing, disassembly, and reverse engineering.

- [ReadELF.jl](https://github.com/JuliaIO/ReadELF.jl) - ELF binary format parser.
- [ObjectFile.jl](https://github.com/JuliaIO/ObjectFile.jl) - Object file format handling.

## Web Security

Web application security testing and analysis.

- [Gumbo.jl](https://github.com/JuliaWeb/Gumbo.jl) - HTML5 parsing for web scraping and analysis.
- [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) - HTTP client for web security testing.
- [URIs.jl](https://github.com/JuliaWeb/URIs.jl) - URI parsing and manipulation.

## Fuzzing

Fuzzing frameworks and mutation testing.

- [Supposition.jl](https://github.com/Seelengrab/Supposition.jl) - Property-based testing for fuzzing.
- [PropCheck.jl](https://github.com/Seelengrab/PropCheck.jl) - Property-based testing framework.

## Security Frameworks

Comprehensive security toolkits and frameworks.

- [Spectra](https://github.com/bad-antics/spectra) - Julia cryptography toolkit with modern algorithms.
- [NullSec Julia Tools](https://github.com/bad-antics/nullsec-juliaprobe) - Security analysis and anomaly detection.

## Learning Resources

Books, courses, and community resources.

### Documentation

- [Julia Security Guide](https://docs.julialang.org/en/v1/manual/security/) - Official security documentation.
- [JuliaCrypto Documentation](https://juliaCrypto.github.io/) - Cryptography package documentation.

### Books

- [Julia High Performance](https://www.packtpub.com/product/julia-high-performance-second-edition/9781788298117) - Performance optimization techniques.
- [Hands-On Design Patterns in Julia](https://www.packtpub.com/product/hands-on-design-patterns-and-best-practices-with-julia/9781838648817) - Design patterns for robust Julia code.

### Communities

- [JuliaCrypto](https://github.com/JuliaCrypto) - Cryptography packages organization.
- [Julia Discourse - Security](https://discourse.julialang.org/c/domain/security) - Security discussions.
- [Julia Slack](https://julialang.org/slack/) - #security channel.

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [bad-antics](https://github.com/bad-antics) has waived all copyright and related or neighboring rights to this work.

## Quantum Computing & Cryptography

Quantum computing frameworks and post-quantum cryptography for Julia.

### Quantum Frameworks

- [Yao.jl](https://github.com/QuantumBFS/Yao.jl) - Extensible, efficient quantum computing framework with quantum circuits.
- [QuantumInformation.jl](https://github.com/iitis/QuantumInformation.jl) - Quantum information theory toolkit.
- [QuantumOptics.jl](https://github.com/qojulia/QuantumOptics.jl) - Library for simulating quantum systems.
- [ITensors.jl](https://github.com/ITensor/ITensors.jl) - Tensor network calculations for quantum simulations.

### Post-Quantum Cryptography

- [NistyPQC.jl](https://github.com/erich-9/NistyPQC.jl) - NIST Post-Quantum Cryptography candidates.
- [Kyber.jl](https://github.com/JuliaCrypto/Kyber.jl) - Kyber lattice-based key encapsulation.
- [CRYSTALS.jl](https://github.com/JuliaCrypto/CRYSTALS.jl) - CRYSTALS-Dilithium signature scheme.

## Reverse Engineering

Binary analysis and reverse engineering tools.

- [LibBFD.jl](https://github.com/Keno/LibBFD.jl) - GNU BFD library bindings for binary parsing.
- [ELF.jl](https://github.com/JuliaInterop/ELF.jl) - ELF file format parser.
- [DWARF.jl](https://github.com/Keno/DWARF.jl) - DWARF debugging information parser.
- [ObjectFile.jl](https://github.com/JuliaIO/ObjectFile.jl) - Object file format handling.
- [Cxx.jl](https://github.com/JuliaInterop/Cxx.jl) - C++ interop for interfacing with RE tools.

## AI/ML Security

Machine learning security and adversarial research.

### Adversarial ML

- [Flux.jl](https://github.com/FluxML/Flux.jl) - ML library suitable for adversarial example generation.
- [Adversarial.jl](https://github.com/jaypmorgan/Adversarial.jl) - Adversarial attack implementations.
- [DifferentialPrivacy.jl](https://github.com/OpenMined/DifferentialPrivacy.jl) - Differential privacy algorithms.

### Model Security

- [ModelAnalysis.jl](https://github.com/JuliaAI/ModelAnalysis.jl) - ML model interpretation and analysis.
- [Interpretability.jl](https://github.com/JuliaAI/Interpretability.jl) - Model interpretability tools.

## Blockchain & Web3

Cryptocurrency and blockchain security tools.

- [Bitcoin.jl](https://github.com/JuliaCrypto/Bitcoin.jl) - Bitcoin protocol implementation.
- [Ethereum.jl](https://github.com/pszufe/Ethereum.jl) - Ethereum interaction library.
- [Secp256k1.jl](https://github.com/JuliaCrypto/Secp256k1.jl) - secp256k1 elliptic curve operations.

## Simulation & Emulation

Security-focused simulation environments.

- [Agents.jl](https://github.com/JuliaDynamics/Agents.jl) - Agent-based modeling for attack simulation.
- [DifferentialEquations.jl](https://github.com/SciML/DifferentialEquations.jl) - System dynamics modeling.
- [StateSpaceModels.jl](https://github.com/LAMPSPUC/StateSpaceModels.jl) - State-space analysis for anomaly detection.

---

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

