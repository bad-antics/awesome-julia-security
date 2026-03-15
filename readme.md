# Awesome Julia Security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of security tools, cryptography libraries, and cybersecurity resources for the Julia programming language.

Julia's high-performance computing capabilities, native parallelism, and scientific computing ecosystem make it uniquely suited for security research, cryptographic implementations, and large-scale threat analysis.

## Contents

- [Cryptography](#cryptography)
  - [Hash Functions](#hash-functions)
  - [Symmetric Encryption](#symmetric-encryption)
  - [Homomorphic Encryption](#homomorphic-encryption)
  - [Post-Quantum Cryptography](#post-quantum-cryptography)
  - [Elliptic Curve Cryptography](#elliptic-curve-cryptography)
  - [Zero-Knowledge Proofs](#zero-knowledge-proofs)
  - [Cryptographic Signatures](#cryptographic-signatures)
  - [Cryptographic Utilities](#cryptographic-utilities)
- [Network Security](#network-security)
  - [Protocol Libraries](#protocol-libraries)
  - [TLS and SSL](#tls-and-ssl)
  - [SSH](#ssh)
  - [Network Reconnaissance](#network-reconnaissance)
  - [GeoIP and DNS](#geoip-and-dns)
- [Web Security](#web-security)
  - [HTTP and Web Frameworks](#http-and-web-frameworks)
  - [Authentication and Tokens](#authentication-and-tokens)
  - [Content Security](#content-security)
- [Binary Analysis and Reverse Engineering](#binary-analysis-and-reverse-engineering)
  - [Binary Formats](#binary-formats)
  - [Debugging and Introspection](#debugging-and-introspection)
  - [Foreign Function Interfaces](#foreign-function-interfaces)
- [Data Forensics and Analysis](#data-forensics-and-analysis)
  - [Data Parsing](#data-parsing)
  - [Database Security](#database-security)
  - [Log Analysis](#log-analysis)
- [Machine Learning for Security](#machine-learning-for-security)
  - [ML Frameworks](#ml-frameworks)
  - [Anomaly and Outlier Detection](#anomaly-and-outlier-detection)
  - [Adversarial ML](#adversarial-ml)
- [Privacy and Anonymity](#privacy-and-anonymity)
  - [Differential Privacy](#differential-privacy)
  - [Secure Voting](#secure-voting)
- [Security Frameworks and Tools](#security-frameworks-and-tools)
  - [Vulnerability Research](#vulnerability-research)
  - [Hash Analysis](#hash-analysis)
  - [Threat Intelligence](#threat-intelligence)
  - [Security Scanning](#security-scanning)
- [Mathematics for Security](#mathematics-for-security)
  - [Number Theory](#number-theory)
  - [Probabilistic Data Structures](#probabilistic-data-structures)
- [Cloud Security](#cloud-security)
- [Resources](#resources)
  - [Documentation](#documentation)
  - [Community](#community)
  - [Conferences and Talks](#conferences-and-talks)
  - [Books and Papers](#books-and-papers)
  - [Security Advisories](#security-advisories)

## Cryptography

### Hash Functions

- [SHA.jl](https://github.com/JuliaCrypto/SHA.jl) - Performant, 100% native-Julia SHA1, SHA2, and SHA3 implementation.
- [MD5.jl](https://github.com/JuliaCrypto/MD5.jl) - Performant, 100% native-Julia MD5 implementation.
- [Ripemd.jl](https://github.com/JuliaCrypto/Ripemd.jl) - Pure Julia RIPEMD-160 implementation.
- [CryptographicHashFunctions.jl](https://github.com/erich-9/CryptographicHashFunctions.jl) - Fast cryptographic hash functions for Julia.
- [Nettle.jl](https://github.com/JuliaCrypto/Nettle.jl) - Libnettle bindings providing MD5, SHA1, SHA2 hashing and HMAC functionality, as well as AES encryption/decryption.

### Symmetric Encryption

- [AES.jl](https://github.com/kanav99/AES.jl) - Advanced Encryption Standard on-the-fly mode implementation in Julia.
- [ChaChaCiphers.jl](https://github.com/kernelmethod/ChaChaCiphers.jl) - GPU-compatible implementations of the ChaCha stream cipher family.
- [SQLCipher.jl](https://github.com/JuliaAPlavin/SQLCipher.jl) - Drop-in replacement for SQLite.jl using the sqlcipher library for full database encryption support.

### Homomorphic Encryption

- [ToyFHE.jl](https://github.com/JuliaCrypto/ToyFHE.jl) - Toy implementation of Fully Homomorphic Encryption algorithms.
- [SEAL.jl](https://github.com/JuliaCrypto/SEAL.jl) - Wrapper for the Microsoft SEAL library supporting homomorphic encryption with BFV and CKKS schemes.
- [OpenFHE.jl](https://github.com/hpsc-lab/OpenFHE.jl) - Julia bindings for OpenFHE, an open-source fully homomorphic encryption library.
- [Paillier.jl](https://github.com/hardbyte/Paillier.jl) - Julia implementation of the Paillier partially homomorphic encryption system.
- [SecureArithmetic.jl](https://github.com/hpsc-lab/SecureArithmetic.jl) - Secure arithmetic operations using fully homomorphic encryption.
- [Carousel.jl](https://github.com/SNUCP/Carousel.jl) - Implementation of Carousel: Fully Homomorphic Encryption from slot blind rotation.
- [FHEW.jl](https://github.com/isentropic/FHEW.jl) - Fully Homomorphic Encryption library in pure Julia.

### Post-Quantum Cryptography

- [NistyPQC.jl](https://github.com/erich-9/NistyPQC.jl) - Post-Quantum Cryptography implementations for Julia based on NIST standards.
- [MKTFHE](https://github.com/SNUCP/MKTFHE) - Implementation of Multi-Key Threshold Fully Homomorphic Encryption.

### Elliptic Curve Cryptography

- [ECC.jl](https://github.com/roshii/ECC.jl) - Elliptic Curve Cryptography in Julia with secp256k1 curve support.
- [CryptoGroups.jl](https://github.com/PeaceFounder/CryptoGroups.jl) - Groups for cryptographic applications including Weierstrass elliptic curves.
- [OpenSSLGroups.jl](https://github.com/PeaceFounder/OpenSSLGroups.jl) - OpenSSL elliptic curve wrapper for CryptoGroups.
- [DarkCurves.jl](https://github.com/nucypher/DarkCurves.jl) - DarkIntegers-based library for working with elliptic curves.

### Zero-Knowledge Proofs

- [Groth.jl](https://github.com/0xpantera/Groth.jl) - Groth16 zkSNARK implementation in Julia, a modular zero-knowledge proof system for learning and research.
- [SigmaProofs.jl](https://github.com/PeaceFounder/SigmaProofs.jl) - Zero-knowledge proofs with practical applications.
- [ShuffleProofs.jl](https://github.com/PeaceFounder/ShuffleProofs.jl) - Verificatum compatible verifier and prover for NIZK proofs of shuffle.

### Cryptographic Signatures

- [CryptoSignatures.jl](https://github.com/PeaceFounder/CryptoSignatures.jl) - Cryptographic signature library supporting DSA and elliptic curve signatures.
- [OpenSSH.jl](https://github.com/JuliaCrypto/OpenSSH.jl) - OpenSSH key generation and management.

### Cryptographic Utilities

- [CryptoUtils.jl](https://github.com/fcasal/CryptoUtils.jl) - Cryptography and number-theory primitives in Julia including continued fractions and prime factoring.
- [CryptoPRG.jl](https://github.com/PeaceFounder/CryptoPRG.jl) - Deterministic pseudorandom generators for cryptographic applications.
- [Krypto.jl](https://github.com/JuliaCrypto/Krypto.jl) - Experimental futuristic crypto library in Julia.
- [ToyPublicKeys.jl](https://github.com/NegaScout/ToyPublicKeys.jl) - Toy implementation of public key cryptography for learning purposes.

## Network Security

### Protocol Libraries

- [HTTP.jl](https://github.com/JuliaWeb/HTTP.jl) - Full-featured HTTP client and server framework for Julia.
- [HTTP2.jl](https://github.com/JuliaWeb/HTTP2.jl) - HTTP/2 protocol implementation for Julia.
- [WebSockets.jl](https://github.com/JuliaWeb/WebSockets.jl) - WebSockets library for Julia, useful for real-time security monitoring dashboards.
- [Sockets.jl](https://docs.julialang.org/en/v1/stdlib/Sockets/) - Standard library for low-level networking and socket programming.
- [ZMQ.jl](https://github.com/JuliaInterop/ZMQ.jl) - Julia interface to ZeroMQ for distributed messaging patterns.

### TLS and SSL

- [MbedTLS.jl](https://github.com/JuliaLang/MbedTLS.jl) - TLS and SSL protocol implementation with certificate management.
- [OpenSSL.jl](https://github.com/JuliaWeb/OpenSSL.jl) - Julia wrapper for OpenSSL cryptographic and TLS functionality.

### SSH

- [LibSSH2.jl](https://github.com/JuliaCloud/LibSSH2.jl) - SSH protocol bindings for secure remote connections.
- [OpenSSH.jl](https://github.com/JuliaCrypto/OpenSSH.jl) - OpenSSH key generation utilities.

### Network Reconnaissance

- [NetProbe](https://github.com/bad-antics/netprobe) - Network reconnaissance and port scanning toolkit with service detection and CIDR support.
- [PacketLib.jl](https://github.com/SamKomesarook/PacketLib.jl) - Packet crafter and packet sniffer library for Julia.

### GeoIP and DNS

- [GeoIP.jl](https://github.com/JuliaWeb/GeoIP.jl) - Estimate the geographic location of IP addresses for threat intelligence geolocation.
- [URIs.jl](https://github.com/JuliaWeb/URIs.jl) - URI parsing and manipulation for web security analysis.

## Web Security

### HTTP and Web Frameworks

- [Mux.jl](https://github.com/JuliaWeb/Mux.jl) - Middleware framework for Julia web applications.
- [JuliaWebAPI.jl](https://github.com/JuliaWeb/JuliaWebAPI.jl) - Package for deploying secure APIs with Julia.
- [Gumbo.jl](https://github.com/JuliaWeb/Gumbo.jl) - Julia wrapper around Google's gumbo HTML parser for web scraping and security analysis.
- [LibCURL.jl](https://github.com/JuliaWeb/LibCURL.jl) - Julia wrapper for libcurl, useful for custom HTTP request crafting.
- [Hyperscript.jl](https://github.com/JuliaWeb/Hyperscript.jl) - Lightweight DOM representation for safe HTML generation.

### Authentication and Tokens

- [JWTs.jl](https://github.com/JuliaWeb/JWTs.jl) - JSON Web Tokens (JWT) implementation for Julia supporting token creation, validation, and verification.
- [GitHub.jl](https://github.com/JuliaWeb/GitHub.jl) - Julia interface for the GitHub API with OAuth authentication support.

### Content Security

- [ContentSecurityPolicy.jl](https://github.com/charlieIT/ContentSecurityPolicy.jl) - Julia library for working with Content Security Policy headers, CSP reports, and XSS mitigation.

## Binary Analysis and Reverse Engineering

### Binary Formats

- [ELF.jl](https://github.com/JuliaInterop/ELF.jl) - ELF binary format parser for Linux executable analysis.
- [MachO.jl](https://github.com/JuliaInterop/MachO.jl) - Mach-O binary format parser for macOS executable analysis.
- [DWARF.jl](https://github.com/JuliaDebug/DWARF.jl) - DWARF debug information parser for binary analysis and reverse engineering.

### Debugging and Introspection

- [Debugger.jl](https://github.com/JuliaDebug/Debugger.jl) - Full-featured Julia debugger for code analysis and vulnerability research.
- [Infiltrator.jl](https://github.com/JuliaDebug/Infiltrator.jl) - No-overhead breakpoints for runtime code inspection.
- [Cthulhu.jl](https://github.com/JuliaDebug/Cthulhu.jl) - Deep code introspection and type-level analysis tool.
- [JuliaInterpreter.jl](https://github.com/JuliaDebug/JuliaInterpreter.jl) - Julia code interpreter for dynamic analysis and security auditing.
- [CodeTracking.jl](https://github.com/JuliaDebug/CodeTracking.jl) - Track method definitions and source locations for code auditing.
- [CassetteOverlay.jl](https://github.com/JuliaDebug/CassetteOverlay.jl) - Method overlay mechanism for instrumenting and intercepting function calls.

### Foreign Function Interfaces

- [Cxx.jl](https://github.com/JuliaInterop/Cxx.jl) - Julia C++ interface for interoperating with native security tools.
- [CxxWrap.jl](https://github.com/JuliaInterop/CxxWrap.jl) - Make C++ security libraries available in Julia.
- [Clang.jl](https://github.com/JuliaInterop/Clang.jl) - C binding generator and interface to libclang for source code analysis.
- [JavaCall.jl](https://github.com/JuliaInterop/JavaCall.jl) - Call Java security libraries from Julia.

## Data Forensics and Analysis

### Data Parsing

- [CSV.jl](https://github.com/JuliaData/CSV.jl) - High-performance CSV file parser for processing log files and data dumps.
- [JSON3.jl](https://github.com/quinnj/JSON3.jl) - High-performance JSON parser for processing API responses and structured data.
- [DataFrames.jl](https://github.com/JuliaData/DataFrames.jl) - Tabular data analysis framework for investigating security events and forensic data.
- [LazyJSON.jl](https://github.com/JuliaCloud/LazyJSON.jl) - Lazy JSON interface for efficiently reading large JSON data files.
- [XMLDict.jl](https://github.com/JuliaCloud/XMLDict.jl) - XML to dictionary parser useful for processing security scan outputs and SAST reports.

### Database Security

- [SQLCipher.jl](https://github.com/JuliaAPlavin/SQLCipher.jl) - Encrypted SQLite database using sqlcipher for secure local data storage.

### Log Analysis

- [SPECTRA](https://github.com/bad-antics/spectra) - Security Protocol Engine for Cyber Threat Response and Analysis with hash analysis, port scanning, pattern detection, and forensics.

## Machine Learning for Security

### ML Frameworks

- [Flux.jl](https://github.com/FluxML/Flux.jl) - Machine learning framework suitable for building anomaly detection models and threat classifiers.
- [MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl) - Machine learning toolbox for building and evaluating security models.
- [Knet.jl](https://github.com/denizyuret/Knet.jl) - Deep learning framework useful for network intrusion detection systems.

### Anomaly and Outlier Detection

- [OutlierDetection.jl](https://github.com/OutlierDetectionJL/OutlierDetection.jl) - Fast, scalable, and flexible outlier detection framework for identifying security anomalies.
- [AnomalyDetection.jl](https://github.com/smidl/AnomalyDetection.jl) - Anomaly detection algorithms for identifying unusual patterns in security data.
- [GenerativeAD.jl](https://github.com/aicenter/GenerativeAD.jl) - Generative models for anomaly detection using deep learning approaches.
- [OutlierDetectionNetworks.jl](https://github.com/OutlierDetectionJL/OutlierDetectionNetworks.jl) - Neural network-based outlier detection algorithms.
- [OutlierDetectionNeighbors.jl](https://github.com/OutlierDetectionJL/OutlierDetectionNeighbors.jl) - Neighbor-based outlier detection algorithms including KNN and LOF.
- [HalfSpaceTrees.jl](https://github.com/e-k-m/HalfSpaceTrees.jl) - Half-space trees for streaming anomaly detection.
- [LinRegOutliers](https://github.com/jbytecode/LinRegOutliers) - Direct and robust methods for outlier detection in linear regression.

### Adversarial ML

- [Mirage](https://github.com/bad-antics/mirage) - Adversarial machine learning toolkit for model extraction, adversarial examples, neural network probing, and defense evaluation.

## Privacy and Anonymity

### Differential Privacy

- [DiffPrivacyInference.jl](https://github.com/DiffMu/DiffPrivacyInference.jl) - Automatically infer differential privacy properties of Julia source code through static analysis.
- [DiffPrivacy.jl](https://github.com/r0cketr1kky/DiffPrivacy.jl) - Library implementing differential privacy techniques over statistical databases.

### Secure Voting

- [PeaceFounder.jl](https://github.com/PeaceFounder/PeaceFounder.jl) - Centralized end-to-end verifiable e-voting system via pseudonym braiding and history trees.
- [ElectionGuardVerifier.jl](https://github.com/mitre/ElectionGuardVerifier.jl) - MITRE Election Guard verifier for secure election auditing.
- [HistoryTrees.jl](https://github.com/PeaceFounder/HistoryTrees.jl) - History tree implementation for tamper-evident logging and audit trails.
- [TallyProofs.jl](https://github.com/PeaceFounder/TallyProofs.jl) - Cryptographic core for end-to-end verifiable voting with everlasting privacy and coercion resistance.

## Security Frameworks and Tools

### Vulnerability Research

- [Phantom](https://github.com/bad-antics/phantom) - Zero-knowledge proof security framework for proving vulnerabilities without revealing details.
- [Oracle](https://github.com/bad-antics/oracle) - AI-powered vulnerability discovery engine using predictive detection with ML models and 300+ patterns.

### Hash Analysis

- [NullSec-HashWitch](https://github.com/bad-antics/nullsec-hashwitch) - High-performance hash identification and cracking tool leveraging Julia's parallel computing.
- [HashForensics](https://github.com/bad-antics/hashforensics) - Hash identification, analysis, and cracking toolkit with 40+ algorithm support.
- [SecureVault](https://github.com/bad-antics/securevault) - Encrypted credential vault with PBKDF2 key derivation, secure memory wiping, and audit logging.

### Threat Intelligence

- [Vortex](https://github.com/bad-antics/vortex) - Real-time threat intelligence fusion engine for correlating IOCs across 50+ feeds with ML analysis.

### Security Scanning

- [RegistryScanner](https://github.com/Octogonapus/RegistryScanner) - Scans Julia registries for possible malicious behavior and misconfigurations.
- [SecurityAdvisories.jl](https://github.com/JuliaLang/SecurityAdvisories.jl) - The official Julia Security Advisory Database.

## Mathematics for Security

### Number Theory

- [Primes.jl](https://github.com/JuliaMath/Primes.jl) - Prime number functions essential for cryptographic key generation and factoring challenges.
- [CryptoUtils.jl](https://github.com/fcasal/CryptoUtils.jl) - Number-theory primitives including continued fractions, modular arithmetic, and prime analysis.

### Probabilistic Data Structures

- [BloomFilters.jl](https://github.com/johnmyleswhite/BloomFilters.jl) - Bloom filter implementation for efficient set membership testing in network security applications.

## Cloud Security

- [AWS.jl](https://github.com/JuliaCloud/AWS.jl) - Julia interface to Amazon Web Services for cloud security automation.
- [AWSAuth.jl](https://github.com/JuliaCloud/AWSAuth.jl) - AWS authentication implementation for secure cloud API access.
- [AWSS3.jl](https://github.com/JuliaCloud/AWSS3.jl) - AWS S3 interface for secure cloud storage operations.
- [GoogleCloud.jl](https://github.com/JuliaCloud/GoogleCloud.jl) - Google Cloud APIs for Julia including IAM and security services.

## Resources

### Documentation

- [Julia Documentation](https://docs.julialang.org) - Official Julia language documentation.
- [Julia Security Policy](https://github.com/JuliaLang/julia/security/policy) - Official Julia security vulnerability reporting process.
- [JuliaCrypto Organization](https://github.com/JuliaCrypto) - Official GitHub organization for Julia cryptography packages.
- [JuliaWeb Organization](https://github.com/JuliaWeb) - Official GitHub organization for Julia web and networking packages.

### Community

- [Julia Discourse - Security](https://discourse.julialang.org) - Community discussion forum with security-related topics.
- [Julia Slack](https://julialang.org/slack/) - Real-time chat community for Julia developers.
- [Julia Zulip](https://julialang.zulipchat.com/) - Zulip chat for Julia development discussions.

### Conferences and Talks

- [JuliaCon](https://juliacon.org/) - Annual Julia conference featuring security and cryptography presentations.
- [JuliaCon YouTube](https://www.youtube.com/c/TheJuliaLanguage) - Recorded conference talks including security-related presentations.
- [Secure Numerical Computations using FHE - JuliaCon 2024](https://github.com/hpsc-lab/talk-2024-juliacon-secure_numerical_computations) - Talk on secure numerical computations using fully homomorphic encryption.

### Books and Papers

- [Secure Numerical Simulations using FHE](https://github.com/hpsc-lab/paper-2024-secure_numerical_simulations) - Research paper and reproducibility repository on secure numerical simulations with homomorphic encryption.
- [Julia for Data Analysis](https://www.manning.com/books/julia-for-data-analysis) - Book covering data analysis techniques applicable to security forensics.

### Security Advisories

- [Julia SecurityAdvisories.jl](https://github.com/JuliaLang/SecurityAdvisories.jl) - Official database of Julia security advisories and vulnerability disclosures.

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.
