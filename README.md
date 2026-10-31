# A Survey of Zero-Knowledge Succinct Non-Interactive Arguments of Knowledge

**Sunkwan Kim**, Northeastern University
kim.sunk@northeastern.edu

**Paper:** [zk-snark-survey.pdf](zk-snark-survey.pdf)

## Abstract

Zero-knowledge succinct non-interactive arguments of knowledge (zk-SNARKs) allow a verifier to check a computation with a proof far shorter than the computation, without learning the prover's private inputs. Over the last decade they have moved from theory to deployed systems, and the number of constructions has grown quickly; with that growth, the term "zk-SNARK" has come to cover schemes with very different guarantees. This survey gives a single formal definition with a strict succinctness requirement and explains the modular pipeline behind most schemes, including lookup arguments, in which the polynomial commitment largely decides the setup, the proof size and the post-quantum status. It then organizes the main construction families by their setup model: circuit-specific trusted setup (GGPR, Pinocchio, Groth16), universal and updatable setup (Sonic, PLONK, Marlin), and transparent setup (Fractal, the random-oracle variant of Spartan, and Supersonic with class groups), with recursion and folding (Halo, Nova) built on top. We compare the schemes in normalized tables of asymptotic costs and setup parameters, with their assumptions and the exact counts the papers report, and give a source for every entry; schemes that are often called zk-SNARKs but miss the strict bound are compared separately. Since 2022 the components have changed more than the families: small and binary fields with challenges from extension fields, lookup-centric and STARK-based zkVMs, folding as an alternative to recursive verification, the gap between proven and conjectured security of hash-based commitments, and lattice-based folding and commitments. We conclude with open problems in prover efficiency and proof size, post-quantum security, recursion overhead and the security of folding, Fiat–Shamir in practice, and SNARGs from standard assumptions, and argue that the schemes meeting the strict definition differ mainly in which of these they trust: a setup, a knowledge assumption or an idealized group model, and a hash function assumed to behave like a random oracle.

## Keywords

zk-SNARKs, Zero-Knowledge Proofs, Polynomial Commitment Schemes, Interactive Oracle Proofs, Sum-Check Protocol, GKR Protocol, Arithmetization, Small and Binary Fields, Fiat–Shamir Transform, Trusted Setup, Recursion and Folding, Lookup Arguments, zkVMs, Proximity Gaps, Post-Quantum Security, Lattice-Based Cryptography

## Contents

1. Introduction
2. Preliminaries
   - 2.1 Notation and mathematical background
   - 2.2 Interactive proofs and arguments
   - 2.3 Cryptographic tools
3. Defining a zk-SNARK
   - 3.1 Why knowledge assumptions and random oracles?
4. Anatomy of a modern zk-SNARK
   - 4.1 Arithmetization
   - 4.2 Information-theoretic protocols: PCPs, IOPs and polynomial IOPs
   - 4.3 Lookup arguments
   - 4.4 Polynomial commitment schemes
   - 4.5 Compiling to a non-interactive argument
5. Construction families of zk-SNARKs
   - 5.1 Circuit-specific setup — GGPR, Pinocchio, Groth16
   - 5.2 Universal and updatable setup — Sonic, PLONK, Marlin
   - 5.3 Transparent setup — Fractal, Spartan, Supersonic (DARK)
   - 5.4 Zero-knowledge arguments outside the strict definition
6. Recursion, accumulation and folding
   - 6.1 Incrementally verifiable computation
   - 6.2 Halo and accumulation schemes
   - 6.3 Folding: Nova
   - 6.4 Generalizations
7. Comparison
8. Developments since 2022
9. Open problems and future directions
   - 9.1 Prover efficiency and proof size
   - 9.2 Post-quantum zk-SNARKs
   - 9.3 Recursion overhead and the security of folding
   - 9.4 Fiat–Shamir in practice
   - 9.5 Foundations: SNARGs from standard assumptions
10. Conclusion

References

Appendix A. Supplementary tables and timeline

## Acknowledgments

This survey is an independent project, conceived and directed by the author without a faculty advisor. AI tools were used to assist in writing this paper.
