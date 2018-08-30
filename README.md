Authenticated Key Exchange in Tamarin
=====================================

This repo contains some models of authenticated key exchange
protocols in the [Tamarin prover](Tamarin)
syntax.

* The BADH protocol from the [SIGMA paper](SIGMA), in order to
  verify that Tamarin finds some known attacks on AKEs.  Identity
  misbinding attacks are manifested as liveness attacks.
* SIGMA itself (without identity protection)
* The [Katz-Yung group AKE compiler](KY07), specialized to a vanilla
  two-party DH exchange.
* A simplified Katz-Yung variant where the DH keys are used as
  entropy instead of dedicated random values.
* An "incremental" Katz-Yung variant that can be done
  asynchronously, and starts to look like an initkey dance...

[Tamarin]: https://tamarin-prover.github.io
[KY07]: http://www.cs.umd.edu/~jkatz/papers/multi-auth-full.pdf
[SIGMA]: http://webee.technion.ac.il/~hugo/sigma-pdf.pdf
