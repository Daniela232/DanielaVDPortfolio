# Academic Programming and Cryptography Projects

This is a public-facing summary of source files provided from academic project archives. Only project descriptions are published here; original archives are **not** redistributed.

## ChaCha20 Stream Cipher and Keystream Reuse — Python
**Files reviewed:** `encrypt.py`, `xor_back.py`, `xor_book.py`, `README.md`.

Implemented an educational demonstration of ChaCha20 encryption and XOR operations on pairs of files. The encryption script derives a key through PBKDF2-HMAC-SHA256 and intentionally uses the **same nonce and key for two inputs**, revealing the security consequences of reusing a stream-cipher keystream. The paired XOR scripts operate on source and encrypted files.

**Security note:** This is an intentionally insecure example designed to illustrate the risk of nonce reuse, not production-ready encryption. The supplied README references script names that differ from the archived source; use the actual source filenames when running it. The supplied source books and output files are excluded from public distribution.

## ECDSA Signatures and Simple Blockchain Data Structure — Python
**Files reviewed:** `generate_keys.py`, `sign_document.py`, `verify_signature.py`, `blockchain.py`.

Implemented demonstration scripts for elliptic-curve P-256 key generation, SHA-256-backed ECDSA signing and verification, and a `Block` data structure with signed data. The provided example generates a keypair without password-encrypting its private key.

**Security note:** The original archive contains a private PEM key and signature artifacts. These are **not published**. Use fresh disposable keys locally for demonstrations.

## Parallel Vector Addition — C++ / OpenMP
**File reviewed:** `OpenMP.cpp`.

Created an OpenMP vector-addition program that distributes array indexes among threads, measures runtime with `omp_get_wtime()`, and validates the expected results. The code requests vector size and number of threads from the user.

## Producer–Consumer Problem — C++ and Python
**Files reviewed:** `ProducerConsumer.cpp`, `ConsumerProducer.py`.

Developed educational producer–consumer simulations using C++ `std::thread` and Python's `threading` module, shared buffers, and configurable input. These examples demonstrate concurrency concepts but **do not implement full synchronization** for shared state; they should not be presented as a thread-safe bounded-buffer implementation.

## Readers–Writers and Synchronization — C++
**Files reviewed:** `CompareandSwapProject3.cpp`, `BinaryCountingSemaphore.cpp`.

Created C++ reader/writer state simulations with atomic variables, compare-and-swap concepts, and a binary-semaphore-themed approach. These are coursework models of synchronization and critical-section access rather than audited production concurrency libraries.

## Publication policy
No private keys, signatures, executables, copyrighted source books, or generated output artifacts are published from the original ZIPs. This repository presents the work accurately without suggesting cryptographic safety or thread safety that the source code does not demonstrate.
