---
description: VDF(Boneh 2018)
---

# Research Direction

## 已经研究的VDF架构

1. 基于模平方计算的Efficient VDF(Wesolowski 2018) 和 Simple VDF(Pietrzak 2019)
2. 基于模平方根计算的Sloth(Lenstra, Wesolowski 2015)
3. 基于椭圆曲线同源映射和双线性映射的Isogency VDF(Feo 2019)

关于Efficient VDF和Simple VDF的综合分析 A Survey of Two Verifiable Delay Functions(Boneh 2018)

关于Efficient VDF和Simple VDF的实现分析 Implementation Study of Two Verifiable Delay Functions(Attias 2020)

## hidden order group VDFs

1. 每一轮结果都可以验证的Continuous VDF(Ephraim 2020) —— 基于Simple VDF
2. 对时间复杂度的严格分析(Döttling 2020) —— 基于Efficient VDF和Simple VDF
3. 分析Fiat-Shamir transform在VDF中的应用(Lombardi 2020) —— 基于Simple VDF
4. 分析low order assumption在虚二次域上的安全性(Belabas 2020) —— 基于Simple VDF
5. 批量验证VDF结果的设计(Rotem 2021) —— 基于Simple VDF
6. 讨论群的阶数一定不可以被泄露 (Rotem 2020)

## other VDFs

1. 最原始的VDF (Boneh 2018)
2. 只使用同源映射而不使用双线性映射的VDF (Shani 2019) —— 基于Isogency VDF
3. 基于random oracle model随机预言机的VDF (Mahmoody 2019)
4. 基于Minimal Circuit Assumptions安全假设的VDF (Jaques 2021)
5. 基于同源映射的抗量子VDF (Chavez-Saab 2021) —— 基于Isogency VDF

## Related

1. TIDE (TIme Delayed Encryption) (Loe 2021)
2. 针对hidden order groups的一系列分析优化 （加速算法、专用硬件、理论分析）
3. low-latency modular multiplication
4. scalable RSA MPC  多方安全计算
5. 零知识证明
6. 随机信标
7. Time-lock Puzzles、Timed-release Crypto、Timed Commitments、Proofs of Sequential Work

## Benchmark

1. VDF-FPGA Implementation of an RSA VDF evaluator targeting FPGAs. 专用硬件的设计
2. Chia VDF competition and implementation
3. Chia VDF Benchmark —— Chia is a blockchain and smart transaction platform based on proofs of space and time rather than proofs of work with other cryptocurrencies. This test profile is benchmarking the CPU performance for Chia VDF performance using the Chia VDF benchmark. The Chia VDF is for the Chia Verifiable Delay Function (Proof of Time).
4. 类似我们的工作，做了多个VDF之间的比较 (Yang Z 2020)

## Reference

Boneh D, Bonneau J, Bünz B, et al. Verifiable delay functions\[C]//Annual international cryptology conference. Springer, Cham, 2018: 757-788.

Wesolowski B. Efficient verifiable delay functions\[C]//Annual International Conference on the Theory and Applications of Cryptographic Techniques. Springer, Cham, 2019: 379-407.

Pietrzak K. Simple verifiable delay functions\[C]//10th innovations in theoretical computer science conference (itcs 2019). Schloss Dagstuhl-Leibniz-Zentrum fuer Informatik, 2018.

Lenstra A K, Wesolowski B. A random zoo: sloth, unicorn, and trx\[J]. Cryptology ePrint Archive, 2015.

De Feo L, Masson S, Petit C, et al. Verifiable delay functions from supersingular isogenies and pairings\[C]//International Conference on the Theory and Application of Cryptology and Information Security. Springer, Cham, 2019: 248-277.

Boneh D, Bünz B, Fisch B. A survey of two verifiable delay functions\[J]. Cryptology ePrint Archive, 2018.

Attias V, Vigneri L, Dimitrov V. Implementation study of two verifiable delay functions\[J]. Cryptology ePrint Archive, 2020.

Ephraim N, Freitag C, Komargodski I, et al. Continuous verifiable delay functions\[C]//Annual International Conference on the Theory and Applications of Cryptographic Techniques. Springer, Cham, 2020: 125-154.

Döttling N, Garg S, Malavolta G, et al. Tight verifiable delay functions\[C]//International Conference on Security and Cryptography for Networks. Springer, Cham, 2020: 65-84.

Lombardi A, Vaikuntanathan V. Fiat-Shamir for repeated squaring with applications to PPAD-hardness and VDFs\[C]//Annual International Cryptology Conference. Springer, Cham, 2020: 632-651.

Belabas K, Kleinjung T, Sanso A, et al. A note on the low order assumption in class group of an imaginary quadratic number fields\[J]. Cryptology ePrint Archive, 2020.

Rotem L. Simple and Efficient Batch Verification Techniques for Verifiable Delay Functions\[C]//Theory of Cryptography Conference. Springer, Cham, 2021: 382-414.

Shani B. A note on isogeny-based hybrid verifiable delay functions\[J]. Cryptology ePrint Archive, 2019.

Mahmoody M, Smith C, Wu D J. Can Verifiable Delay Functions be Based on Random Oracles?\[J]. Cryptology ePrint Archive, 2019.

Rotem L, Segev G, Shahaf I. Generic-group delay functions require hidden-order groups\[C]//Annual International Conference on the Theory and Applications of Cryptographic Techniques. Springer, Cham, 2020: 155-180.

Jaques S, Montgomery H, Rosie R, et al. Time-release cryptography from minimal circuit assumptions\[C]//International Conference on Cryptology in India. Springer, Cham, 2021: 584-606.

Chavez-Saab J, Henríquez F R, Tibouchi M. Verifiable Isogeny Walks: Towards an Isogeny-based Postquantum VDF\[J]. Cryptology ePrint Archive, 2021.

Loe A F, Medley L, O’Connell C, et al. A Practical Verifiable Delay Function and Delay Encryption Scheme\[J]. Cryptology ePrint Archive, 2021.

Yang Z, Qin B, Wu Q, et al. Experimental Comparisons of Verifiable Delay Functions\[C]//International Conference on Information and Communications Security. Springer, Cham, 2020: 510-527.

