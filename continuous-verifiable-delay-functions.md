---
description: CCF A-EUROCRYPT
---

# Continuous Verifiable Delay Functions

&#x20;想要做到每一轮计算的结果都可以被验证

a **continuous verifiable delay function** (cVDF). As the name suggests, it can be viewed as enabling continuous evaluation and verification of a verifiable delay function

the construction of a cVDF based on the repeated squaring assumption in a finite group of unknown order and a variant of the Fiat-Shamir (FS) heuristic for constant-round proof systems. Informally, the iteratively sequential property of our construction comes from the repeated squaring assumption which says that squaring in this setting is an iteratively sequential function. We use the Fiat-Shamir assumption to obtain the continuous verifiability property of our construction. More precisely, we apply the Fiat-Shamir heuristic on a constant-round proof system where the verifier may be inefficient.

This suggests a high-level framework for making the construction continuous: starting at the root where we want to compute x2t , recursively compute and prove each of the three sub-instances. Specifically, each step of the cVDF will be a step in the traversal of this tree. At any point when all three sub-instances of a node have been proven, merge the proofs into a proof of the parent node and “forget” the proofs of the sub-instances. This has the two desirable properties we want for a cVDF—first, at any point a new party can verify the state before continuing the computation, since the state only contains the nodes that have been completed; second, due to the structure of the proofs, the proof size at any node is bounded roughly by the height of the tree and hence avoids a blowup in verification time.
