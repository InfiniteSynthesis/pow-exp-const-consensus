<h1 align="center">Proof-of-Work-based Consensus<br/>in Expected-Constant Time</h1>

<p align="center">
Juan Garay<sup>1</sup>, Aggelos Kiayias<sup>2,3</sup>, Yu Shen<sup>2</sup>
</p>

<p align="center">
<sup>1</sup>Texas A&M University
<sup>2</sup>University of Edinburgh
<sup>3</sup>IOG
</p>

<p align="center">
    <a href="http://creativecommons.org/licenses/by/4.0/"><img src="https://img.shields.io/badge/License-CC--BY--4.0-bb6688.svg?style=for-the-badge&labelColor=884499" alt="License"></a>
    <a href="https://link.springer.com/chapter/10.1007/978-3-031-58734-4_4"><img src="https://img.shields.io/badge/Proceedings-EUROCRYPT 2024-8888cc.svg?style=for-the-badge&labelColor=884499" alt="Proceedings"></a>
    <a href="https://eprint.iacr.org/2023/1663"><img src="https://img.shields.io/badge/Full-Version-ccaa88.svg?style=for-the-badge&labelColor=884499" alt="Full Version"></a>
</p>

> [!NOTE]  
> This repository contains the LaTeX source code of "Proof-of-Work-Based Consensus in Expected-Constant Time." An abridged version of this paper appears in *Proc. EUROCRYPT 2024*.

## :books: Abstract

In the traditional consensus problem (aka Byzantine agreement), parties are required to agree on a common value despite the malicious behavior of some of them, subject to the condition that if all the honest parties start the execution with the same value, then that should be the outcome. This problem has been extensively studied by both the distributed computing and cryptographic protocols communities. With the advent of blockchains, whose main application—a distributed ledger—essentially requires that miners agree on their views, new techniques have been proposed to solve the problem, and in particular in so-called "permissionless" environments, where parties are not authenticated or have access to point-to-point channels and, further, may come and go as they please.

So far, the fastest way to achieve consensus in the proof-of-work (PoW)-based setting of Bitcoin, takes $O(\mathsf{polylog} \kappa)$ number of rounds, where $\kappa$ is the security parameter. We present the first protocol in this setting that requires expected-constant number of rounds. Furthermore, we show how to apply securely sequential composition in order to yield a fast distributed ledger protocol that settles all transactions in expected-constant time. Our result is based on a novel instantiation of "m-for-1 PoWs" on parallel chains that facilitates our basic building block, Chain-King Consensus. The techniques we use, via parallel chains, to port classical protocol design elements (such as Phase-King Consensus, super-phase sequential composition and others) into the permissionless setting may be of independent interest.
