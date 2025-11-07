# NIST SP 800‑90C: Random Bit Generator Constructions

Cryptographic systems rely on random numbers for generating keys, nonces and
other values.  If the randomness is weak, attackers may predict keys and
break security.  NIST’s **SP 800‑90C** recommends constructions for
**random bit generators (RBGs)** that combine deterministic algorithms with
sources of true entropy【652213821792537†L119-L137】.

## Four classes of constructions

1. **RBG1:** Uses an external random bit generator to initialize a
   deterministic random bit generator (DRBG).  After the initial seeding,
   the DRBG produces pseudorandom bits without further entropy input.
2. **RBG2:** Includes a source of entropy that can be requested on demand.
   The DRBG periodically mixes fresh entropy into its state【652213821792537†L119-L137】.
3. **RBG3:** Incorporates a continuously available entropy source.  This
   design is suitable when hardware can provide a steady stream of random
   bits【652213821792537†L119-L137】.
4. **RBGC:** Allows chaining multiple RBGs to build stronger generators.
   For example, one generator can seed another, or generators can be run
   in parallel to produce higher throughput【652213821792537†L119-L137】.

## Why the document is important

SP 800‑90C completes the SP 800‑90 series on random number generation.  By
standardizing how deterministic algorithms and entropy sources are
combined, it helps developers design RBGs that are both practical and
secure.  Organizations implementing cryptographic systems should ensure
that their RBGs follow one of the approved constructions so that the
resulting random bits are unpredictable and suitable for security
applications【652213821792537†L119-L137】.
