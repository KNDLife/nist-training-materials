# NIST Post‑Quantum Cryptography Standards: FIPS 203, SP 800‑227, FIPS 204 & FIPS 205

Quantum computers pose a threat to current cryptographic algorithms.  To
prepare for a future where adversaries may have quantum capabilities, NIST
has issued new standards for **post‑quantum cryptography (PQC)**.

## FIPS 203 – Module‑Lattice‑Based Key‑Encapsulation Mechanism (ML‑KEM)

FIPS 203 specifies **ML‑KEM**, a key‑encapsulation mechanism used to
establish a shared secret over an untrusted channel.  Its security is based
on the computational hardness of the **Module Learning with Errors (MLWE)**
problem.  The standard defines three parameter sets—**ML‑KEM‑512,
ML‑KEM‑768 and ML‑KEM‑1024**—which offer increasing security strength and
trade off performance accordingly【32614351790063†L135-L163】.

## SP 800‑227 – Recommendations for Key‑Encapsulation Mechanisms

SP 800‑227 provides guidance on implementing key‑encapsulation mechanisms,
including ML‑KEM.  The initial draft was released in early 2025, with a
comment period and a public workshop【96603190612650†L119-L137】.
The final publication (September 2025) incorporates feedback and offers
recommendations on selecting parameter sets, handling keys securely and
integrating KEMs into systems【268166394428535†L119-L132】.

## FIPS 204 – Module‑Lattice‑Based Digital Signature Standard (ML‑DSA)

FIPS 204 defines **ML‑DSA**, a digital signature scheme derived from the
CRYSTALS‑Dilithium submission.  Digital signatures allow a signer to
authenticate a message and prevent repudiation.  ML‑DSA leverages lattice
cryptography to remain secure against quantum adversaries【477617157629473†L135-L160】.

## FIPS 205 – Stateless Hash‑Based Digital Signature Standard (SLH‑DSA)

FIPS 205 specifies **SLH‑DSA**, a stateless hash‑based signature scheme
based on **SPHINCS+**.  Like ML‑DSA, it ensures that signatures remain
verifiable even with powerful quantum computers.  The scheme does not
require maintaining state between signatures, which simplifies
implementation【319122553630203†L129-L153】.

## Why these standards matter

Adopting post‑quantum algorithms now gives organizations time to test and
transition before quantum computers become practical.  ML‑KEM, ML‑DSA and
SLH‑DSA provide strong security foundations based on hard mathematical
problems.  SP 800‑227 helps implementers use these mechanisms correctly.
Together, they represent a critical step toward a quantum‑resistant
cryptographic ecosystem【32614351790063†L135-L163】【268166394428535†L119-L132】.
