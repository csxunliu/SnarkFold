# SnarkFold
SnarkFold: A novel proof aggregation scheme based on the folding scheme

# Introduction
SnarkFold is a novel SNARK-proof aggregation scheme based on the folding scheme proposed in [Nova](https://par.nsf.gov/servlets/purl/10440508). It offers constant aggregated proof size and constant verification time. SnarkFold adopts a novel concept of incremental verification (IV), which is derived from incrementally verifiable computation (IVC) but tailored for proof aggregation.

SnarkFold is considered a verification-friendly scheme as the verifier only needs to validate the IV proof of the final recursive step, and the size of an IV proof is independent of the number of recursions.

This library implemented SnarkFold for Plonk in Rust with BN254/Grumpkin, a half-pairing cycle of elliptic curves.

# Details of the library
1. Implement the folding scheme for Plonk proof relation.
2. Construct the recursive circuit for generating IV Proof.
3. Implement a SNARK based on [Spartan](https://eprint.iacr.org/2019/550.pdf), to produce the final IV proof.




