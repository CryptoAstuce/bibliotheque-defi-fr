# Bibliothèque DeFi et blockchain en français

397 parcours de lecture de code, en français, sur des protocoles DeFi, des rollups, des bridges, des projets ZK, Bitcoin, NFT, Base et Hyperliquid, pour un total de 3212 chapitres.

Chaque parcours suit le code source d'un projet open source réel. On part du dépôt officiel, on lit les contrats ou le code dans l'ordre où ils s'exécutent, et on explique chaque mécanisme en français. Les noms de fichiers et de fonctions sont donnés pour pouvoir tout vérifier soi-même.

## Comment lire un parcours

- Chaque lien « lire » ouvre la branche du dépôt où le parcours est publié. Le README de cette branche indique où se trouvent les chapitres, en général dans `docs/fr/`.
- La colonne « Licence du code » est celle du projet étudié, pas celle du parcours. Vérifiez-la avant de réutiliser ce code.
- Un parcours décrit le code à la date où il a été écrit. Le projet a pu évoluer depuis.

## Avertissement

Ces parcours ont été rédigés avec l'aide d'une IA, à partir de la lecture du code. La plupart n'ont pas été vérifiés en exécutant ce code, et chaque parcours précise ce qui a été testé. Ce ne sont ni des audits de sécurité ni des conseils d'investissement. Si vous trouvez une erreur, ouvrez une issue sur ce dépôt.

## Sommaire

- [Hyperliquid](#hyperliquid) (18)
- [Recherche transversale](#recherche-transversale) (9)
- [ZK et FHE](#zk-et-fhe) (47)
- [Bitcoin](#bitcoin) (15)
- [Base](#base) (75)
- [NFT](#nft) (16)
- [Stablecoins](#stablecoins) (12)
- [Prêt, emprunt et crédit](#prêt-emprunt-et-crédit) (27)
- [Staking et restaking](#staking-et-restaking) (14)
- [Échanges : DEX, intents et market making](#échanges--dex-intents-et-market-making) (49)
- [Dérivés, options et marchés prédictifs](#dérivés-options-et-marchés-prédictifs) (18)
- [Vaults, rendement et gestion d'actifs](#vaults-rendement-et-gestion-dactifs) (12)
- [Bridges et interopérabilité](#bridges-et-interopérabilité) (15)
- [Comptes, wallets et identité](#comptes-wallets-et-identité) (11)
- [Oracles, paiements et automatisation](#oracles-paiements-et-automatisation) (16)
- [DAO et gouvernance](#dao-et-gouvernance) (3)
- [Ethereum, rollups et infrastructure](#ethereum-rollups-et-infrastructure) (40)

## Hyperliquid

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [caliperforge/hyperevm-safety](https://github.com/caliperforge/hyperevm-safety) | HyperEVM Safety (oracles HyperCore, decimales, solvabilite, liquidations et invariants adverses) | Apache-2.0 | 5 | [lire](https://github.com/CryptoAstuce/hyperevm-safety/tree/main) |
| [circlefin/hyperevm-circle-contracts](https://github.com/circlefin/hyperevm-circle-contracts) | Circle HyperEVM Contracts (CoreDepositWallet, CCTP, CREATE2 et proxies) | Apache-2.0 | 5 | [lire](https://github.com/studiokvc/hyperevm-circle-contracts/tree/master) |
| [emo-eth/hyperevm-tools](https://github.com/emo-eth/hyperevm-tools) | HyperEVM Tools (L1Read, L1Write, CoreWriter, transferts cross-DEX et fixtures) | MIT | 6 | [lire](https://github.com/HereForTheTechNFT/hyperevm-tools/tree/main) |
| [hyperlendx/hyperevm-oracle](https://github.com/hyperlendx/hyperevm-oracle) | HyperLend HyperEVM Oracle (System Oracle, interface Chainlink, keepers, EMA et fraicheur) | à vérifier | 8 | [lire](https://github.com/Crypt0-Gr0wth/hyperevm-oracle/tree/master) |
| [hyperliquid-dev/hyper-evm-lib](https://github.com/hyperliquid-dev/hyper-evm-lib) | hyper-evm-lib (CoreWriter, precompiles, conversions, ponts HyperCore et checklist d integration) | MIT | 10 | [lire](https://github.com/JulienKervarrec/hyper-evm-lib/tree/main) |
| [hyperliquid-dex/block-importer](https://github.com/hyperliquid-dex/block-importer) | Block Importer (pipeline HyperEVM, ordre, reprise, idempotence et integrite) | à vérifier | 4 | [lire](https://github.com/Crypt0-Gr0wth/block-importer/tree/main) |
| [hyperliquid-dex/contracts](https://github.com/hyperliquid-dex/contracts) | Hyperliquid Contracts (Bridge2, signatures, anti-rejeu et frontiere de confiance) | à vérifier | 9 | [lire](https://github.com/artofbitcoin/hyperliquid-contracts/tree/master) |
| [hyperliquid-dex/historical_data](https://github.com/hyperliquid-dex/historical_data) | Hyperliquid Historical Data (trades non-MM, liquidations, ledger et controle qualite) | à vérifier | 8 | [lire](https://github.com/JulienKervarrec/historical_data/tree/master) |
| [hyperliquid-dex/hyper-evm-sync](https://github.com/hyperliquid-dex/hyper-evm-sync) | HyperEVM Sync (rejeu historique, etats, snapshots, integrite, precompiles et reprise) | à vérifier | 5 | [lire](https://github.com/HereForTheTechNFT/hyper-evm-sync/tree/main) |
| [hyperliquid-dex/hyperliquid-python-sdk](https://github.com/hyperliquid-dex/hyperliquid-python-sdk) | Hyperliquid Python SDK (Info, Exchange, signatures, nonces, ordres et reconciliation) | MIT | 5 | [lire](https://github.com/HereForTheTechNFT/hyperliquid-python-sdk/tree/master) |
| [hyperliquid-dex/hyperliquid-rust-sdk](https://github.com/hyperliquid-dex/hyperliquid-rust-sdk) | Hyperliquid Rust SDK (signatures, ordres, nonces, websocket et reconciliation) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/hyperliquid-rust-sdk/tree/master) |
| [hyperliquid-dex/hyperliquid-stats](https://github.com/hyperliquid-dex/hyperliquid-stats) | Hyperliquid Stats (ingestion, idempotence, metriques, cache et fraicheur) | à vérifier | 5 | [lire](https://github.com/DigitalA7/hyperliquid-stats/tree/main) |
| [hyperliquid-dex/hyperliquid-stats-web](https://github.com/hyperliquid-dex/hyperliquid-stats-web) | Hyperliquid Stats Web (provenance des metriques, flux React, volumes, cache et fraicheur) | MIT | 8 | [lire](https://github.com/CryptoAstuce/hyperliquid-stats-web/tree/main) |
| [hyperliquid-dex/node](https://github.com/hyperliquid-dex/node) | Hyperliquid Node (roles, RPC HyperEVM, Info local, flux, provenance, rattrapage et retention) | Apache-2.0 | 8 | [lire](https://github.com/creativityventures/node/tree/main) |
| [hyperliquid-dex/order_book_server](https://github.com/hyperliquid-dex/order_book_server) | Order Book Server (evenements du noeud, carnet L4, WebSocket et auto-verification) | MIT | 5 | [lire](https://github.com/artofbitcoin/order_book_server/tree/main) |
| [hyperliquid-dex/ts-examples](https://github.com/hyperliquid-dex/ts-examples) | Hyperliquid TypeScript Examples (decimales, liquidation, ordres, signatures et frontiere HyperEVM) | MIT | 5 | [lire](https://github.com/cryptokvc/ts-examples/tree/main) |
| [nktkas/hyperliquid](https://github.com/nktkas/hyperliquid) | Hyperliquid TypeScript SDK (transports, signatures, ordres, websocket et HyperEVM) | MIT | 5 | [lire](https://github.com/A5Infinity/hyperliquid/tree/main) |
| [sand0vvv/hyperevm-mcp](https://github.com/sand0vvv/hyperevm-mcp) | HyperEVM MCP (lecture seule, SSRF, texte hostile, donnees manquantes, cache et audit mecanique) | MIT | 6 | [lire](https://github.com/creativityventures/hyperevm-mcp/tree/main) |

## Recherche transversale

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [A5Infinity/A5Infinity](https://github.com/A5Infinity/A5Infinity) | A5Infinity (preuves ZK, FHE, architecture Base, FHEVM, HyperEVM et sécurité EVM) | à vérifier | 76 | [lire](https://github.com/A5Infinity/A5Infinity/tree/main) |
| [artofbitcoin/artofbitcoin](https://github.com/artofbitcoin/artofbitcoin) | artofbitcoin (Bitcoin, actifs représentés, Base, HyperEVM, Hyperliquid, ZK et FHE) | à vérifier | 62 | [lire](https://github.com/artofbitcoin/artofbitcoin/tree/main) |
| [creativityventures/creativityventures](https://github.com/creativityventures/creativityventures) | creativityventures (invariants, preuves ZK, accès FHE, agents Base et indexation Hyperliquid) | à vérifier | 73 | [lire](https://github.com/creativityventures/creativityventures/tree/main) |
| [Crypt0-Gr0wth/Crypt0-Gr0wth](https://github.com/Crypt0-Gr0wth/Crypt0-Gr0wth) | Crypt0-Gr0wth (preuves ZK, confidentialité FHE, politiques Base et intégrité Hyperliquid) | à vérifier | 67 | [lire](https://github.com/Crypt0-Gr0wth/Crypt0-Gr0wth/tree/main) |
| [CryptoAstuce/CryptoAstuce](https://github.com/CryptoAstuce/CryptoAstuce) | CryptoAstuce (STARK, FHE, Base, HyperEVM, provenance et audit reproductible) | à vérifier | 95 | [lire](https://github.com/CryptoAstuce/CryptoAstuce/tree/main) |
| [cryptokvc/cryptokvc](https://github.com/cryptokvc/cryptokvc) | cryptokvc (preuves ZK, FHEVM, architecture Base, signatures EVM et intégrité Hyperliquid) | à vérifier | 63 | [lire](https://github.com/cryptokvc/cryptokvc/tree/main) |
| [DigitalA7/DigitalA7](https://github.com/DigitalA7/DigitalA7) | Digital A7 (preuves ZK, FHE, Base, HyperEVM, DeFi et sécurité des smart contracts) | à vérifier | 48 | [lire](https://github.com/DigitalA7/DigitalA7/tree/main) |
| [HereForTheTechNFT/HereForTheTechNFT](https://github.com/HereForTheTechNFT/HereForTheTechNFT) | Here For The Tech (Base, HyperEVM, Hyperliquid, FHE, STARK et ZK-NFT) | à vérifier | 73 | [lire](https://github.com/HereForTheTechNFT/HereForTheTechNFT/tree/main) |
| [studiokvc/studiokvc](https://github.com/studiokvc/studiokvc) | Studio KVC (ZK, FHE, Base, HyperEVM, DeFi, interopérabilité et méthode documentaire) | à vérifier | 58 | [lire](https://github.com/studiokvc/studiokvc/tree/main) |

## ZK et FHE

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [0xMiden/air-script](https://github.com/0xMiden/air-script) | AirScript (DSL AIR, parser, MIR, AirIR, codegen Winterfell et recursion ACE) | MIT | 5 | [lire](https://github.com/JulienKervarrec/air-script/tree/next) |
| [0xMiden/crypto](https://github.com/0xMiden/crypto) | Miden Crypto (hachages algebriques, Merkle, transcript, aleatoire et AEAD) | MIT / Apache-2.0 | 5 | [lire](https://github.com/CryptoAstuce/crypto/tree/next) |
| [0xMiden/miden-vm](https://github.com/0xMiden/miden-vm) | Miden VM (execution, traces, AIR, preuves STARK et precompiles) | MIT / Apache-2.0 | 5 | [lire](https://github.com/A5Infinity/miden-vm/tree/next) |
| [0xPolygonZero/plonky2](https://github.com/0xPolygonZero/plonky2) | Plonky2 (Goldilocks, contraintes PLONK, engagements Merkle, FRI et recursion) | MIT / Apache-2.0 | 5 | [lire](https://github.com/HereForTheTechNFT/plonky2/tree/main) |
| [arkworks-rs/algebra](https://github.com/arkworks-rs/algebra) | arkworks algebra (corps finis, groupes, courbes elliptiques, pairings, polynomes, hash-to-curve et serialization) | MIT / Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/algebra/tree/master) |
| [arkworks-rs/groth16](https://github.com/arkworks-rs/groth16) | ark-groth16 (R1CS, parametres, preuve, appairages et checklist d integration) | MIT / Apache-2.0 | 5 | [lire](https://github.com/HereForTheTechNFT/groth16/tree/master) |
| [arkworks-rs/marlin](https://github.com/arkworks-rs/marlin) | Marlin (SRS universel, indexation, AHP et engagements polynomiaux) | MIT / Apache-2.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/marlin/tree/master) |
| [arkworks-rs/poly-commit](https://github.com/arkworks-rs/poly-commit) | Arkworks Poly-Commit (KZG, Marlin, IPA, Hyrax, Ligero, Brakedown et batching) | MIT / Apache-2.0 | 5 | [lire](https://github.com/JulienKervarrec/poly-commit/tree/master) |
| [arkworks-rs/r1cs-std](https://github.com/arkworks-rs/r1cs-std) | r1cs-std (allocations, booleens, champs, comparaisons, conversions et gadgets cryptographiques) | MIT / Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/r1cs-std/tree/master) |
| [arkworks-rs/r1cs-tutorial](https://github.com/arkworks-rs/r1cs-tutorial) | Arkworks R1CS Tutorial (contraintes, signatures Schnorr, Merkle et transition d etat d un mini-rollup) | MIT OR Apache-2.0 | 8 | [lire](https://github.com/DigitalA7/r1cs-tutorial/tree/main) |
| [axiom-crypto/halo2-lib](https://github.com/axiom-crypto/halo2-lib) | Axiom halo2-lib (gates, range checks, SafeType, arithmetique non native, ECC et pairings) | MIT | 5 | [lire](https://github.com/CryptoAstuce/halo2-lib/tree/main) |
| [aztecprotocol/aztec-packages](https://github.com/aztecprotocol/aztec-packages) | Aztec | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/aztec-packages/tree/next) |
| [boundless-xyz/boundless](https://github.com/boundless-xyz/boundless) | Boundless (marché de preuves, requêtes, broker, assessors et fulfillment) | à vérifier | 4 | [lire](https://github.com/HereForTheTechNFT/boundless/tree/main) |
| [Consensys-Incorporated/gnark](https://github.com/Consensys-Incorporated/gnark) | gnark (circuits, contraintes, Groth16, PLONK, courbes, export Solidity et audits) | Apache-2.0 | 6 | [lire](https://github.com/JulienKervarrec/gnark-fr/tree/master) |
| [Consensys-Incorporated/gnark](https://github.com/Consensys-Incorporated/gnark) | gnark (circuits Go, R1CS/SCS, Groth16, PLONK et verification EVM) | Apache-2.0 | 5 | [lire](https://github.com/studiokvc/gnark/tree/master) |
| [facebook/winterfell](https://github.com/facebook/winterfell) | Winterfell (trace Fibonacci, AIR, transcript, FRI et politique de verification) | MIT | 11 | [lire](https://github.com/JulienKervarrec/winterfell/tree/main) |
| [FhenixProtocol/cofhe-miniapp-template](https://github.com/FhenixProtocol/cofhe-miniapp-template) | CoFHE MiniApp Template (calcul chiffre, permissions, decryption et MiniApp Base) | MIT | 5 | [lire](https://github.com/artofbitcoin/cofhe-miniapp-template/tree/master) |
| [FhenixProtocol/cofhesdk](https://github.com/FhenixProtocol/cofhesdk) | CoFHE SDK (chiffrement, permissions, decryption, React et mocks) | à vérifier | 5 | [lire](https://github.com/A5Infinity/cofhesdk/tree/master) |
| [homenc/HElib](https://github.com/homenc/HElib) | HElib (BGV, CKKS, packing SIMD, bruit et bootstrapping) | Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/HElib/tree/master) |
| [iden3/circom](https://github.com/iden3/circom) | Circom (compilateur de circuits, contraintes R1CS, temoins C++ et WebAssembly, simplification et analyse statique) | GPL-3.0 | 10 | [lire](https://github.com/studiokvc/circom/tree/master) |
| [iden3/snarkjs](https://github.com/iden3/snarkjs) | snarkjs (Groth16, PLONK, FFLONK, temoin, fullprove et verification EVM) | GPL-3.0 | 11 | [lire](https://github.com/JulienKervarrec/snarkjs/tree/master) |
| [JulienKervarrec/zk-research](https://github.com/JulienKervarrec/zk-research) | ZK Research (depot original : diagnostics Winterfell et preconditions des retraits Base) | à vérifier | 7 | [lire](https://github.com/JulienKervarrec/zk-research/tree/main) |
| [lambdaclass/lambdaworks](https://github.com/lambdaclass/lambdaworks) | Lambdaworks (trace, AIR, composition, FRI, Merkle, R1CS et engagements polynomiaux) | MIT / Apache-2.0 | 5 | [lire](https://github.com/creativityventures/lambdaworks/tree/main) |
| [microsoft/SEAL](https://github.com/microsoft/SEAL) | Microsoft SEAL (BFV, BGV, CKKS, batching, niveaux, serialisation et securite) | MIT | 5 | [lire](https://github.com/JulienKervarrec/SEAL/tree/main) |
| [microsoft/SEAL-Embedded](https://github.com/microsoft/SEAL-Embedded) | Microsoft SEAL-Embedded (chiffrement BFV embarque, adapter, RNS/NTT et provisionnement) | MIT | 5 | [lire](https://github.com/CryptoAstuce/SEAL-Embedded/tree/main) |
| [noir-lang/noir](https://github.com/noir-lang/noir) | Noir (pipeline HIR/SSA, ACIR, ACVM, Brillig, Nargo et backends de preuve) | MIT OR Apache-2.0 | 10 | [lire](https://github.com/DigitalA7/noir/tree/master) |
| [openfheorg/openfhe-development](https://github.com/openfheorg/openfhe-development) | OpenFHE (BFV, BGV, CKKS, FHEW/TFHE, bruit et bootstrapping) | BSD-2-Clause | 5 | [lire](https://github.com/studiokvc/openfhe-development/tree/main) |
| [Plonky3/Plonky3](https://github.com/Plonky3/Plonky3) | Plonky3 (AIR, traces, MMCS, FRI, Fiat-Shamir et verification STARK) | MIT OR Apache-2.0 | 8 | [lire](https://github.com/DigitalA7/Plonky3/tree/main) |
| [privacy-ethereum/halo2](https://github.com/privacy-ethereum/halo2) | Halo2 (circuits, contraintes, colonnes, regions, gates, lookups, transcripts et verification) | MIT / Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/halo2/tree/main) |
| [risc0/risc0](https://github.com/risc0/risc0) | RISC Zero (zkVM RV32IM, recus STARK, recursion et Groth16 EVM) | Apache-2.0 | 5 | [lire](https://github.com/cryptokvc/risc0/tree/main) |
| [scroll-tech/scroll](https://github.com/scroll-tech/scroll) | Scroll (zkEVM, rollup, lots, prover, coordinator, pont L1/L2 et observabilite) | MIT | 8 | [lire](https://github.com/JulienKervarrec/scroll-fr/tree/develop) |
| [scroll-tech/zkvm-prover](https://github.com/scroll-tech/zkvm-prover) | Scroll zkVM Prover (chunks, batches, bundles, recursion STARK, verification SNARK EVM, engagements de programme) | MIT / Apache-2.0 | 10 | [lire](https://github.com/A5Infinity/zkvm-prover/tree/master) |
| [semaphore-protocol/semaphore](https://github.com/semaphore-protocol/semaphore) | Semaphore (identite anonyme, groupes, arbre de Merkle, preuves d appartenance et nullifiers) | MIT | 8 | [lire](https://github.com/JulienKervarrec/semaphore/tree/main) |
| [starkware-libs/cairo](https://github.com/starkware-libs/cairo) | Cairo | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/cairo/tree/main) |
| [starkware-libs/proving](https://github.com/starkware-libs/proving) | StarkWare Proving (Cairo AIR, Circle STARK, FRI, recursion et serialisation) | Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/proving/tree/main) |
| [starkware-libs/stone-prover](https://github.com/starkware-libs/stone-prover) | Stone Prover (CPU AIR CairoZero, Merkle, FRI et parametres de securite) | Apache-2.0 | 5 | [lire](https://github.com/studiokvc/stone-prover/tree/main) |
| [starkware-libs/stwo](https://github.com/starkware-libs/stwo) | STWO (Circle STARK, AIR, composition, FRI et transcript) | Apache-2.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/stwo/tree/dev) |
| [succinctlabs/sp1](https://github.com/succinctlabs/sp1) | SP1 (zkVM RISC-V, AIR, FRI, recursion et enveloppes Groth16/PLONK) | MIT / Apache-2.0 | 5 | [lire](https://github.com/artofbitcoin/sp1/tree/main) |
| [taikoxyz/taiko-mono](https://github.com/taikoxyz/taiko-mono) | Taiko Alethia (based rollup, origines L1, propositions, preuves, clients, pont et signaux) | MIT / GPL-3.0 selon les composants | 6 | [lire](https://github.com/CryptoAstuce/taiko-mono/tree/main) |
| [unionlabs/union](https://github.com/unionlabs/union) | Union (light clients, messages, canaux, preuves, relayers, finalite et anti-replay) | Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/union/tree/main) |
| [worldcoin/world-id-contracts](https://github.com/worldcoin/world-id-contracts) | World ID Contracts (identité unique, preuves, nullifiers et scopes) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/world-id-contracts/tree/main) |
| [zama-ai/concrete](https://github.com/zama-ai/concrete) | Concrete (compilation FHE, graphes, bruit, parametres et frontieres de confiance) | BSD-3-Clause-Clear | 4 | [lire](https://github.com/Crypt0-Gr0wth/concrete/tree/main) |
| [zama-ai/fhevm](https://github.com/zama-ai/fhevm) | FHEVM (handles chiffres, ACL, coprocesseur, KMS, gateway et modele de menace) | BSD-3-Clause-Clear | 5 | [lire](https://github.com/HereForTheTechNFT/fhevm/tree/main) |
| [zama-ai/fhevm-react-template](https://github.com/zama-ai/fhevm-react-template) | FHEVM React Template (types chiffres, ACL, relais et decryption) | BSD-3-Clause-Clear | 5 | [lire](https://github.com/cryptokvc/fhevm-react-template/tree/main) |
| [zama-ai/tfhe-rs](https://github.com/zama-ai/tfhe-rs) | TFHE-rs (ciphertexts, bootstrap programmable, entiers chiffres, parametres et modele de menace) | BSD-3-Clause-Clear | 5 | [lire](https://github.com/creativityventures/tfhe-rs/tree/main) |
| [zcash/halo2](https://github.com/zcash/halo2) | Halo 2 (circuits, contraintes, lookups, engagements et transcript) | MIT / Apache-2.0 | 5 | [lire](https://github.com/A5Infinity/halo2/tree/main) |
| [zkcrypto/bellman](https://github.com/zkcrypto/bellman) | Bellman (R1CS, Groth16, parametres, temoins et verification) | MIT / Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/bellman/tree/main) |

## Bitcoin

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [ACINQ/eclair](https://github.com/ACINQ/eclair) | Eclair (canaux, routage, paiements et persistance) | Apache-2.0 | 4 | [lire](https://github.com/JulienKervarrec/eclair/tree/master) |
| [Bitcoin-ABC/bitcoin-abc](https://github.com/Bitcoin-ABC/bitcoin-abc) | Bitcoin ABC | à vérifier | 6 | [lire](https://github.com/artofbitcoin/bitcoin-abc/tree/master) |
| [bitcoin-core/secp256k1](https://github.com/bitcoin-core/secp256k1) | libsecp256k1 (clés, ECDSA, Schnorr et calcul constant) | MIT | 4 | [lire](https://github.com/JulienKervarrec/secp256k1/tree/master) |
| [bitcoin/bitcoin](https://github.com/bitcoin/bitcoin) | Bitcoin | à vérifier | 6 | [lire](https://github.com/artofbitcoin/bitcoin/tree/master) |
| [bitcoindevkit/bdk](https://github.com/bitcoindevkit/bdk) | Bitcoin Dev Kit (descripteurs, adresses, transactions, synchronisation et persistance) | MIT / Apache-2.0 | 4 | [lire](https://github.com/JulienKervarrec/bdk/tree/master) |
| [bitcoinjs/bitcoinjs-lib](https://github.com/bitcoinjs/bitcoinjs-lib) | Bibliotheque Bitcoin | à vérifier | 6 | [lire](https://github.com/artofbitcoin/bitcoinjs-lib/tree/master) |
| [blockstream/esplora](https://github.com/blockstream/esplora) | Indexation Bitcoin | à vérifier | 6 | [lire](https://github.com/artofbitcoin/esplora/tree/master) |
| [btcsuite/btcd](https://github.com/btcsuite/btcd) | Noeud Bitcoin Go | à vérifier | 6 | [lire](https://github.com/artofbitcoin/btcd/tree/master) |
| [ElementsProject/elements](https://github.com/ElementsProject/elements) | Elements (actifs émis, peg Bitcoin, valeurs confidentielles et validation) | MIT | 4 | [lire](https://github.com/JulienKervarrec/elements/tree/master) |
| [ElementsProject/lightning](https://github.com/ElementsProject/lightning) | Core Lightning (BOLT, canaux, HTLC, routage, factures et plugins) | BSD-3-Clause / MIT | 4 | [lire](https://github.com/JulienKervarrec/lightning/tree/master) |
| [fedimint/fedimint](https://github.com/fedimint/fedimint) | Fedimint (consensus fédéré, modules, ecash, peg et Lightning) | MIT | 4 | [lire](https://github.com/JulienKervarrec/fedimint/tree/master) |
| [lightningnetwork/lnd](https://github.com/lightningnetwork/lnd) | LND (canaux, HTLC, routage, paiements en oignon et RPC) | MIT | 4 | [lire](https://github.com/JulienKervarrec/lnd/tree/master) |
| [mempool/mempool](https://github.com/mempool/mempool) | Mempool Bitcoin | à vérifier | 6 | [lire](https://github.com/artofbitcoin/mempool/tree/master) |
| [ordinals/ord](https://github.com/ordinals/ord) | Ordinals / Runes | à vérifier | 6 | [lire](https://github.com/artofbitcoin/ord/tree/master) |
| [rust-bitcoin/rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin) | rust-bitcoin (transactions, scripts, blocs, consensus et signatures) | CC0-1.0 | 4 | [lire](https://github.com/JulienKervarrec/rust-bitcoin/tree/master) |

## Base

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [aerodrome-finance/contracts](https://github.com/aerodrome-finance/contracts) | Aerodrome (pools stables et volatiles, veAERO, gauges, votes, emissions, bribes et gouvernance) | Apache-2.0 | 7 | [lire](https://github.com/JulienKervarrec/aerodrome-contracts/tree/main) |
| [base/account-policies](https://github.com/base/account-policies) | account-policies (PolicyManager wallet-agnostique installant des modules de policy a capacite restreinte sur un compte, cycle de vie install/execute/uninstall/replace, pattern SingleExecutorAuthorizedPolicy) | MIT | 6 | [lire](https://github.com/JulienKervarrec/account-policies/tree/main) |
| [base/account-sdk](https://github.com/base/account-sdk) | Base Account SDK (provider EIP-1193, popup Communicator, chiffrement ECDH/AES-GCM, sous-comptes, Base Pay, subscriptions EIP-712) | MIT | 18 | [lire](https://github.com/JulienKervarrec/account-sdk/tree/master) |
| [base/account-sdk](https://github.com/base/account-sdk) | Base Account SDK (provider EIP-1193, popup Communicator, chiffrement ECDH/AES-GCM, sous-comptes, Base Pay, subscriptions EIP-712) | MIT | 13 | [lire](https://github.com/CryptoAstuce/account-sdk/tree/master) |
| [base/base](https://github.com/base/base) | Base Node / Base components | à vérifier | 10 | [lire](https://github.com/A5Infinity/base/tree/main) |
| [base/base](https://github.com/base/base) | Base | à vérifier | 8 | [lire](https://github.com/studiokvc/base/tree/main) |
| [base/base](https://github.com/base/base) | Base | à vérifier | 13 | [lire](https://github.com/cryptokvc/base/tree/main) |
| [base/base](https://github.com/base/base) | Base | à vérifier | 8 | [lire](https://github.com/artofbitcoin/base/tree/main) |
| [base/base](https://github.com/base/base) | Base | MIT | 7 | [lire](https://github.com/CryptoAstuce/base/tree/main) |
| [base/base](https://github.com/base/base) | Base (clients execution et rollup, derivation L1, blobs, finalite et fault proofs) | MIT | 25 | [lire](https://github.com/JulienKervarrec/base/tree/main) |
| [base/base-anvil](https://github.com/base/base-anvil) | Base Anvil | à vérifier | 7 | [lire](https://github.com/A5Infinity/base-anvil/tree/base-anvil-fork) |
| [base/base-anvil](https://github.com/base/base-anvil) | Base Anvil | à vérifier | 8 | [lire](https://github.com/studiokvc/base-anvil/tree/base-anvil-fork) |
| [base/base-anvil](https://github.com/base/base-anvil) | Base Anvil | à vérifier | 8 | [lire](https://github.com/cryptokvc/base-anvil/tree/base-anvil-fork) |
| [base/base-anvil](https://github.com/base/base-anvil) | Base Anvil | à vérifier | 8 | [lire](https://github.com/artofbitcoin/base-anvil/tree/base-anvil-fork) |
| [base/base-anvil](https://github.com/base/base-anvil) | Base Anvil | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/base-anvil/tree/base-anvil-fork) |
| [base/base-std](https://github.com/base/base-std) | Base Std | à vérifier | 7 | [lire](https://github.com/A5Infinity/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | Base Std | à vérifier | 8 | [lire](https://github.com/studiokvc/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | Base Std | à vérifier | 8 | [lire](https://github.com/cryptokvc/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | Base Std | à vérifier | 8 | [lire](https://github.com/artofbitcoin/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | Base Std (bibliotheque de precompiles Solidity pour Base : P256, RIP-7212, gestion des adresses systeme) | MIT | 25 | [lire](https://github.com/JulienKervarrec/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | Base Std (bibliotheque de precompiles Solidity pour Base : Factory/Policy Registry/Activation Registry, standard de token B20) | MIT | 13 | [lire](https://github.com/CryptoAstuce/base-std/tree/main) |
| [base/base-std](https://github.com/base/base-std) | base-std (L1Block, Superchain, P256/passkeys et integration defensive) | MIT | 9 | [lire](https://github.com/HereForTheTechNFT/base-std/tree/main) |
| [base/basenames](https://github.com/base/basenames) | Base Names | à vérifier | 11 | [lire](https://github.com/studiokvc/basenames/tree/main) |
| [base/benchmark](https://github.com/base/benchmark) | Base Benchmark | à vérifier | 8 | [lire](https://github.com/studiokvc/benchmark/tree/main) |
| [base/benchmark](https://github.com/base/benchmark) | Base Benchmark | à vérifier | 8 | [lire](https://github.com/cryptokvc/benchmark/tree/main) |
| [base/benchmark](https://github.com/base/benchmark) | Base Benchmark | à vérifier | 8 | [lire](https://github.com/artofbitcoin/benchmark/tree/main) |
| [base/benchmark](https://github.com/base/benchmark) | Base Benchmark | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/benchmark/tree/main) |
| [base/blob-archiver](https://github.com/base/blob-archiver) | blob-archiver (service Archiver + API qui archive de maniere permanente les blobs du beacon chain au-dela de leur fenetre de retention native et les rend interrogeables via une API compatible) | MIT | 6 | [lire](https://github.com/JulienKervarrec/blob-archiver/tree/master) |
| [base/bridge](https://github.com/base/bridge) | Base Bridge | à vérifier | 8 | [lire](https://github.com/A5Infinity/bridge/tree/main) |
| [base/bridge](https://github.com/base/bridge) | Base Bridge | à vérifier | 8 | [lire](https://github.com/studiokvc/bridge/tree/main) |
| [base/bridge](https://github.com/base/bridge) | Base Bridge | à vérifier | 8 | [lire](https://github.com/cryptokvc/bridge/tree/main) |
| [base/bridge](https://github.com/base/bridge) | Base Bridge | à vérifier | 8 | [lire](https://github.com/artofbitcoin/bridge/tree/main) |
| [base/bridge](https://github.com/base/bridge) | Base Bridge | MIT | 5 | [lire](https://github.com/CryptoAstuce/bridge/tree/main) |
| [base/commerce-payments](https://github.com/base/commerce-payments) | Commerce Payments Protocol (authorize/capture/void/refund en escrow, TokenStore par operateur, ERC-3009, Permit2, PreApproval, SpendPermission) | MIT | 18 | [lire](https://github.com/JulienKervarrec/commerce-payments/tree/main) |
| [base/commerce-payments](https://github.com/base/commerce-payments) | Commerce Payments Protocol (authorize/capture/void/refund en escrow, TokenStore par operateur, ERC-3009, Permit2, PreApproval, SpendPermission) | MIT | 13 | [lire](https://github.com/CryptoAstuce/commerce-payments/tree/main) |
| [base/contract-deployments](https://github.com/base/contract-deployments) | Base Contract Deployments | à vérifier | 11 | [lire](https://github.com/studiokvc/contract-deployments/tree/main) |
| [base/contracts](https://github.com/base/contracts) | Base Contracts | à vérifier | 11 | [lire](https://github.com/studiokvc/contracts/tree/main) |
| [base/contracts](https://github.com/base/contracts) | Base Contracts (messagerie L1/L2, depots, retraits, bridge et gouvernance) | MIT | 5 | [lire](https://github.com/artofbitcoin/contracts/tree/main) |
| [base/demos](https://github.com/base/demos) | Base Demos | à vérifier | 6 | [lire](https://github.com/A5Infinity/demos/tree/master) |
| [base/demos](https://github.com/base/demos) | Base Demos | à vérifier | 8 | [lire](https://github.com/studiokvc/demos/tree/master) |
| [base/demos](https://github.com/base/demos) | Base Demos | à vérifier | 8 | [lire](https://github.com/cryptokvc/demos/tree/master) |
| [base/demos](https://github.com/base/demos) | Base Demos | à vérifier | 8 | [lire](https://github.com/artofbitcoin/demos/tree/master) |
| [base/demos](https://github.com/base/demos) | Base Demos | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/demos/tree/master) |
| [base/dispute-game-tool](https://github.com/base/dispute-game-tool) | dispute-game-tool (script Python d incident lisant le storage brut d une DisputeGameFactory pour determiner, apres une divergence de client, la liste des dispute games a blacklister) | à vérifier | 4 | [lire](https://github.com/JulienKervarrec/dispute-game-tool/tree/master) |
| [base/docs](https://github.com/base/docs) | Base Docs | à vérifier | 6 | [lire](https://github.com/A5Infinity/docs/tree/master) |
| [base/docs](https://github.com/base/docs) | Base Docs | à vérifier | 8 | [lire](https://github.com/studiokvc/docs/tree/master) |
| [base/docs](https://github.com/base/docs) | Base Docs | à vérifier | 7 | [lire](https://github.com/cryptokvc/docs/tree/master) |
| [base/docs](https://github.com/base/docs) | Base Docs | à vérifier | 8 | [lire](https://github.com/artofbitcoin/docs/tree/master) |
| [base/docs](https://github.com/base/docs) | Base Docs | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/docs/tree/master) |
| [base/eip-7702-proxy](https://github.com/base/eip-7702-proxy) | eip-7702-proxy (proxy ERC-1967 gerant la mise a niveau securisee d un EOA delegue par EIP-7702 vers une implementation de smart wallet, avec NonceTracker et validateur d etat de compte) | MIT | 6 | [lire](https://github.com/JulienKervarrec/eip-7702-proxy/tree/main) |
| [base/eip-8130](https://github.com/base/eip-8130) | EIP-8130 | à vérifier | 6 | [lire](https://github.com/A5Infinity/eip-8130/tree/main) |
| [base/eip-8130](https://github.com/base/eip-8130) | EIP-8130 | à vérifier | 8 | [lire](https://github.com/studiokvc/eip-8130/tree/main) |
| [base/eip-8130](https://github.com/base/eip-8130) | EIP-8130 | à vérifier | 8 | [lire](https://github.com/cryptokvc/eip-8130/tree/main) |
| [base/eip-8130](https://github.com/base/eip-8130) | EIP-8130 | à vérifier | 8 | [lire](https://github.com/artofbitcoin/eip-8130/tree/main) |
| [base/eip-8130](https://github.com/base/eip-8130) | EIP-8130 sur Base | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/eip-8130/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Nitro Validator | à vérifier | 8 | [lire](https://github.com/studiokvc/nitro-validator/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Nitro Validator | à vérifier | 8 | [lire](https://github.com/cryptokvc/nitro-validator/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Nitro Validator | à vérifier | 8 | [lire](https://github.com/artofbitcoin/nitro-validator/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Base Nitro Validator | à vérifier | 8 | [lire](https://github.com/CryptoAstuce/nitro-validator/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Nitro Validator (CBOR/COSE, certificats, P-384, fraicheur, rejeu et revocation) | MIT | 5 | [lire](https://github.com/creativityventures/nitro-validator/tree/main) |
| [base/op-enclave](https://github.com/base/op-enclave) | op-enclave (modification de l op-stack qui prouve les transitions d etat dans une enclave AWS Nitro et supprime la periode de contestation de 7 jours, retraits immediats) | MIT | 6 | [lire](https://github.com/JulienKervarrec/op-enclave/tree/main) |
| [base/op-enclave](https://github.com/base/op-enclave) | op-enclave (Nitro, mesures, politique PCR, derivation et provenance L1) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/op-enclave/tree/main) |
| [base/paymaster](https://github.com/base/paymaster) | paymaster (contrat verifiant qui sponsorise le gas des UserOperations ERC-4337, clone du VerifyingPaymaster eth-infinitism, plus paquet Go de signature) | GPL-3.0 | 11 | [lire](https://github.com/JulienKervarrec/paymaster/tree/main) |
| [base/rollup-boost](https://github.com/base/rollup-boost) | rollup-boost (sidecar Rust qui multiplexe les appels Engine API entre op-geth local et un builder de blocs externe, avec validation, repli automatique et coupure a chaud) | MIT | 6 | [lire](https://github.com/JulienKervarrec/rollup-boost/tree/main) |
| [base/skills](https://github.com/base/skills) | Base Skills (reseau, Base Account, paiements, ERC-8021 et agents) | à vérifier | 5 | [lire](https://github.com/studiokvc/skills/tree/master) |
| [base/skills](https://github.com/base/skills) | Base Skills (frontieres L2, comptes, paiements, ERC-8021 et agents) | à vérifier | 5 | [lire](https://github.com/DigitalA7/skills/tree/master) |
| [base/triedb](https://github.com/base/triedb) | triedb (base de donnees embarquee Rust stockant le trie d etat Ethereum en Pages de 4 Ko organisees selon la structure du trie, MVCC par copie sur ecriture) | MIT | 6 | [lire](https://github.com/JulienKervarrec/triedb/tree/main) |
| [base/webauthn-sol](https://github.com/base/webauthn-sol) | webauthn-sol (bibliotheque Solidity de verification de signatures WebAuthn/secp256r1, RIP-7212 avec repli FreshCryptoLib) | MIT | 6 | [lire](https://github.com/JulienKervarrec/webauthn-sol/tree/main) |
| [base/withdrawer](https://github.com/base/withdrawer) | withdrawer (preuve et finalisation des retraits ETH depuis les chaines op-stack vers Ethereum L1, avec ou sans fault proofs) | MIT | 13 | [lire](https://github.com/JulienKervarrec/withdrawer/tree/main) |
| [base/withdrawer](https://github.com/base/withdrawer) | withdrawer (preuve et finalisation des retraits ETH depuis les chaines op-stack vers Ethereum L1, avec ou sans fault proofs) | MIT | 8 | [lire](https://github.com/CryptoAstuce/withdrawer/tree/main) |
| [bunnyos/base-agent](https://github.com/bunnyos/base-agent) | BunnyOS Base Agent (provenance, sessions, injection, approbation et moindre privilege) | AGPL-3.0 | 8 | [lire](https://github.com/Crypt0-Gr0wth/base-agent/tree/main) |
| [coinbase/agentkit](https://github.com/coinbase/agentkit) | Coinbase AgentKit (wallets, actions typees, MCP, injection de prompt et politiques de transaction) | Apache-2.0 | 8 | [lire](https://github.com/creativityventures/agentkit/tree/main) |
| [coinbase/verifying-paymaster](https://github.com/coinbase/verifying-paymaster) | Coinbase Verifying Paymaster (EntryPoint v0.7, signatures, bundlers, ERC-20 et griefing) | MIT | 6 | [lire](https://github.com/artofbitcoin/verifying-paymaster/tree/master) |
| [nervosnetwork/ckb](https://github.com/nervosnetwork/ckb) | Nervos CKB (Cell Model, CKB-VM RISC-V, scripts, PoW, nœud, stockage et migrations) | MIT | 6 | [lire](https://github.com/JulienKervarrec/ckb-fr/tree/develop) |
| [Savjee/SavjeeCoin](https://github.com/Savjee/SavjeeCoin) | Chaine de blocs minimale (PoW, signatures ECDSA) | MIT | 7 | [lire](https://github.com/DigitalA7/SavjeeCoin/tree/master) |

## NFT

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [ArtBlocks/artblocks-contracts](https://github.com/ArtBlocks/artblocks-contracts) | Art Blocks (GenArt721, projects, scripts, randomizer, minters et royalties) | LGPL-3.0 | 6 | [lire](https://github.com/HereForTheTechNFT/artblocks-contracts/tree/main) |
| [chiru-labs/ERC721A](https://github.com/chiru-labs/ERC721A) | ERC721A | à vérifier | 6 | [lire](https://github.com/A5Infinity/ERC721A/tree/main) |
| [decentraland/land](https://github.com/decentraland/land) | Decentraland LAND (parcelles, Estates, fingerprints et opérateurs) | Apache-2.0 | 4 | [lire](https://github.com/A5Infinity/land/tree/master) |
| [erc6551/reference](https://github.com/erc6551/reference) | ERC-6551 reference (token bound accounts, registry et bytecode déterministe) | MIT | 5 | [lire](https://github.com/creativityventures/reference/tree/main) |
| [immutable/contracts](https://github.com/immutable/contracts) | Immutable Contracts (presets ERC721/ERC1155/ERC20, bridging, marketplace, AMM et wallets) | Apache-2.0 | 6 | [lire](https://github.com/DigitalA7/contracts/tree/main) |
| [looksrare/contracts-exchange-v1](https://github.com/looksrare/contracts-exchange-v1) | LooksRare Exchange v1 (ordres, stratégies, monnaies et exécution) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/contracts-exchange-v1/tree/master) |
| [manifoldxyz/creator-core-solidity](https://github.com/manifoldxyz/creator-core-solidity) | Manifold Creator Core | à vérifier | 6 | [lire](https://github.com/A5Infinity/creator-core-solidity/tree/main) |
| [NFTX-project/nftx-protocol-v2](https://github.com/NFTX-project/nftx-protocol-v2) | NFTX Protocol v2 (vaults, dépôts, redemption et staking) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/nftx-protocol-v2/tree/master) |
| [nounsDAO/nouns-monorepo](https://github.com/nounsDAO/nouns-monorepo) | Nouns DAO | à vérifier | 6 | [lire](https://github.com/HereForTheTechNFT/nouns-monorepo/tree/master) |
| [ourzora/zora-protocol](https://github.com/ourzora/zora-protocol) | Zora Protocol | à vérifier | 6 | [lire](https://github.com/HereForTheTechNFT/zora-protocol/tree/main) |
| [partydao/partybid](https://github.com/partydao/partybid) | PartyBid | à vérifier | 6 | [lire](https://github.com/cryptokvc/partybid/tree/main) |
| [ProjectOpenSea/seaport](https://github.com/ProjectOpenSea/seaport) | Seaport (ordres offer/consideration, zones, conduits, ordres de contrat) | MIT | 15 | [lire](https://github.com/CryptoAstuce/seaport/tree/main) |
| [rarible/protocol-contracts](https://github.com/rarible/protocol-contracts) | Rarible Protocol | à vérifier | 6 | [lire](https://github.com/HereForTheTechNFT/protocol-contracts/tree/master) |
| [sudoswap/lssvm2](https://github.com/sudoswap/lssvm2) | sudoAMM (pools NFT, courbes de prix, inventaire et frais) | GPL-3.0 | 4 | [lire](https://github.com/A5Infinity/lssvm2/tree/main) |
| [unlock-protocol/unlock](https://github.com/unlock-protocol/unlock) | Unlock Protocol (PublicLock, keys, expirations, hooks, pricing et fees) | MIT | 6 | [lire](https://github.com/HereForTheTechNFT/unlock/tree/master) |
| [unlock-protocol/unlock](https://github.com/unlock-protocol/unlock) | Unlock Protocol (locks, clés NFT, accès et abonnements) | MIT | 4 | [lire](https://github.com/A5Infinity/unlock/tree/master) |

## Stablecoins

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [AngleProtocol/angle-core](https://github.com/AngleProtocol/angle-core) | Angle Core Module (stablecoin, collatéral, gouvernance et surplus) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/angle-core/tree/main) |
| [AngleProtocol/angle-transmuter](https://github.com/AngleProtocol/angle-transmuter) | Angle Transmuter (stabilité, collatéral, oracle et couverture) | BUSL-1.1 / GPL | 4 | [lire](https://github.com/cryptokvc/angle-transmuter/tree/main) |
| [curvefi/curve-stablecoin](https://github.com/curvefi/curve-stablecoin) | Curve Stablecoin (crvUSD, LLAMMA, Llamalend, oracles EMA, liquidations progressives, zaps et flashloans) | MIT | 8 | [lire](https://github.com/JulienKervarrec/curve-stablecoin-fr/tree/master) |
| [ethena-labs/code4arena-contest](https://github.com/ethena-labs/code4arena-contest) | Ethena USDtb (ordres signés, whitelist, blacklist et états de transfert) | MIT | 4 | [lire](https://github.com/cryptokvc/code4arena-contest/tree/main) |
| [fei-protocol/fei-protocol-core](https://github.com/fei-protocol/fei-protocol-core) | Fei Protocol (stablecoin, PCV, oracles et rate limits) | MIT | 5 | [lire](https://github.com/creativityventures/fei-protocol-core/tree/develop) |
| [fraxfinance/frax-solidity](https://github.com/fraxfinance/frax-solidity) | Frax Solidity (stablecoins, Fraxswap, bonds, BAMM et staking) | MIT | 5 | [lire](https://github.com/creativityventures/frax-solidity/tree/master) |
| [liquity/dev](https://github.com/liquity/dev) | Liquity (troves, LUSD, Stability Pool et rachats) | GPL-2.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/dev/tree/main) |
| [makerdao/dss](https://github.com/makerdao/dss) | MakerDAO DSS | à vérifier | 11 | [lire](https://github.com/creativityventures/dss/tree/master) |
| [mento-protocol/mento-core](https://github.com/mento-protocol/mento-core) | Mento Core (stablecoins Celo, réserves et market makers à prix fixe) | GPL-3.0 | 4 | [lire](https://github.com/studiokvc/mento-core/tree/develop) |
| [OriginProtocol/origin-dollar](https://github.com/OriginProtocol/origin-dollar) | Origin Dollar OUSD/OETH (rebasing, vault et stratégies) | MIT | 4 | [lire](https://github.com/cryptokvc/origin-dollar/tree/master) |
| [prisma-fi/prisma-contracts](https://github.com/prisma-fi/prisma-contracts) | Prisma Finance (mkUSD, positions, LST et Stability Pool) | MIT | 4 | [lire](https://github.com/A5Infinity/prisma-contracts/tree/main) |
| [reserve-protocol/protocol](https://github.com/reserve-protocol/protocol) | Reserve Protocol (RTokens, paniers de collatéraux, stRSR, émission, rachat et rééquilibrage) | MIT | 5 | [lire](https://github.com/HereForTheTechNFT/protocol/tree/master) |

## Prêt, emprunt et crédit

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [aave/aave-v3-core](https://github.com/aave/aave-v3-core) | Aave v3 (aTokens a solde scale, taux a deux pentes, eMode, mode isole, liquidations, flash loans) | à vérifier | 18 | [lire](https://github.com/CryptoAstuce/aave-v3-core/tree/master) |
| [aave/aave-v3-periphery](https://github.com/aave/aave-v3-periphery) | Aave V3 Periphery (passerelles, récompenses et fournisseurs de données) | BUSL-1.1 | 4 | [lire](https://github.com/JulienKervarrec/aave-v3-periphery/tree/master) |
| [ajna-finance/ajna-core](https://github.com/ajna-finance/ajna-core) | Ajna (pools, buckets, dette, positions et liquidations) | BUSL-1.1 | 6 | [lire](https://github.com/HereForTheTechNFT/ajna-core/tree/master) |
| [centrifuge/liquidity-pools](https://github.com/centrifuge/liquidity-pools) | Centrifuge Liquidity Pools (pools, vaults ERC-7540, permissions et multi-chaînes) | Apache-2.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/liquidity-pools/tree/main) |
| [code-423n4/2024-06-size](https://github.com/code-423n4/2024-06-size) | Size Protocol (prêts à taux fixe et marchés de maturité) | MIT | 4 | [lire](https://github.com/cryptokvc/2024-06-size/tree/main) |
| [compound-finance/comet](https://github.com/compound-finance/comet) | Compound v3 / Comet (marche monetaire mono-collateral de base, modele de taux a double pente, recompenses) | BUSL-1.1 (Business Source License) | 13 | [lire](https://github.com/creativityventures/comet/tree/main) |
| [compound-finance/compound-protocol](https://github.com/compound-finance/compound-protocol) | Compound v2 (cTokens, taux algorithmiques, liquidation) | BSD-3-Clause | 14 | [lire](https://github.com/JulienKervarrec/compound-protocol/tree/master) |
| [euler-xyz/ethereum-vault-connector](https://github.com/euler-xyz/ethereum-vault-connector) | Ethereum Vault Connector (sous-comptes, collatéraux, contrôleurs et contrôles différés) | GPL-2.0-or-later | 4 | [lire](https://github.com/JulienKervarrec/ethereum-vault-connector/tree/master) |
| [euler-xyz/euler-vault-kit](https://github.com/euler-xyz/euler-vault-kit) | Euler Vault Kit / EVK (vaults ERC-4626 modulaires par delegatecall, Ethereum Vault Connector, IRM pluggable, liquidation avec socialisation) | à vérifier | 13 | [lire](https://github.com/Crypt0-Gr0wth/euler-vault-kit/tree/master) |
| [exactly/protocol](https://github.com/exactly/protocol) | Exactly Protocol (marches a taux variable et fixe, Market, Auditor, maturites, liquidations et proxies) | MIT | 8 | [lire](https://github.com/JulienKervarrec/protocol/tree/main) |
| [Gearbox-protocol/core-v3](https://github.com/Gearbox-protocol/core-v3) | Gearbox V3 (Credit Accounts, adaptateurs, exécution, risque et liquidation) | BUSL-1.1 | 4 | [lire](https://github.com/artofbitcoin/core-v3/tree/main) |
| [gitcoinco/grants-stack](https://github.com/gitcoinco/grants-stack) | Gitcoin Grants Stack | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/grants-stack/tree/main) |
| [goldfinch-eng/goldfinch-contracts](https://github.com/goldfinch-eng/goldfinch-contracts) | Goldfinch (adhésion, pools, tranches et crédit) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/goldfinch-contracts/tree/main) |
| [goldfinch-eng/mono](https://github.com/goldfinch-eng/mono) | Goldfinch (pools de crédit, borrowers, tranched pools et underwriting) | MIT | 4 | [lire](https://github.com/HereForTheTechNFT/mono/tree/main) |
| [Instadapp/fluid-contracts-public](https://github.com/Instadapp/fluid-contracts-public) | Instadapp Fluid (vaults, collatéral, liquidations et liquidité) | BUSL-1.1 | 4 | [lire](https://github.com/Crypt0-Gr0wth/fluid-contracts-public/tree/main) |
| [Kamino-Finance/klend](https://github.com/Kamino-Finance/klend) | Kamino KLend (marchés, collatéral, dette, taux et liquidation) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/klend/tree/master) |
| [morpho-org/morpho-blue](https://github.com/morpho-org/morpho-blue) | Morpho Blue (marches de pret isoles, immuables et sans gouvernance, SharesMathLib anti-inflation) | GPL-2.0-or-later | 13 | [lire](https://github.com/creativityventures/morpho-blue/tree/main) |
| [morpho-org/morpho-blue](https://github.com/morpho-org/morpho-blue) | Morpho Blue (marches isoles, parts, interets, collaterale et liquidation) | GPL-2.0-or-later | 12 | [lire](https://github.com/studiokvc/morpho-blue/tree/main) |
| [morpho-org/morpho-blue](https://github.com/morpho-org/morpho-blue) | Morpho Blue (marchés permissionless, dépôts, emprunts, solvabilité et liquidation) | GPL-2.0-or-later | 6 | [lire](https://github.com/artofbitcoin/morpho-blue/tree/main) |
| [notional-finance/contracts-v3](https://github.com/notional-finance/contracts-v3) | Notional V3 (marches fCash a taux fixe, Prime Cash / Prime Debt a taux variable, coffres a effet de levier) | à vérifier | 13 | [lire](https://github.com/Crypt0-Gr0wth/contracts-v3/tree/master-v3) |
| [paxoslabs/ion-protocol](https://github.com/paxoslabs/ion-protocol) | Ion Protocol (marchés de prêt, collatéral staké, taux et liquidations) | MIT | 4 | [lire](https://github.com/A5Infinity/ion-protocol/tree/master) |
| [PoolTogether/v4-periphery](https://github.com/PoolTogether/v4-periphery) | PoolTogether V4 Periphery (tirages, prix, sponsors et distributions) | GPL-3.0 | 4 | [lire](https://github.com/cryptokvc/v4-periphery/tree/master) |
| [pooltogether/v5-vault](https://github.com/pooltogether/v5-vault) | PoolTogether V5 Vault (ERC-4626, contributions et chances de gain) | MIT | 4 | [lire](https://github.com/JulienKervarrec/v5-vault/tree/main) |
| [sky-ecosystem/dss](https://github.com/sky-ecosystem/dss) | MakerDAO / Sky Protocol dss (CDP Vat, taux de stabilite Jug, liquidations 2.0 Dog/Clip, epargne DSR Pot, reglement global End) | AGPL-3.0-or-later | 13 | [lire](https://github.com/HereForTheTechNFT/dss/tree/master) |
| [solendprotocol/public](https://github.com/solendprotocol/public) | Solend Public (SDK, client léger et liquidateur) | à vérifier | 5 | [lire](https://github.com/DigitalA7/public/tree/master) |
| [TrueFi-Protocol/contracts-ragnarok](https://github.com/TrueFi-Protocol/contracts-ragnarok) | TrueFi (portefeuilles de crédit, prêts, remboursements et gouvernance) | MIT | 4 | [lire](https://github.com/A5Infinity/contracts-ragnarok/tree/main) |
| [VenusProtocol/venus-protocol](https://github.com/VenusProtocol/venus-protocol) | Venus Protocol (vTokens, Comptroller Diamond, taux, liquidations et gouvernance) | à vérifier | 5 | [lire](https://github.com/artofbitcoin/venus-protocol/tree/develop) |

## Staking et restaking

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [code-423n4/2023-06-stader](https://github.com/code-423n4/2023-06-stader) | Stader (ETHx, validateurs, oracle et récompenses) | MIT | 4 | [lire](https://github.com/cryptokvc/2023-06-stader/tree/main) |
| [code-423n4/2024-04-renzo](https://github.com/code-423n4/2024-04-renzo) | Renzo (ezETH, opérateurs, dépôts et retraits) | MIT | 4 | [lire](https://github.com/studiokvc/renzo-audit/tree/main) |
| [etherfi-protocol/smart-contracts](https://github.com/etherfi-protocol/smart-contracts) | ether.fi (liquid restaking via eETH/weETH, restaking natif EigenPod, file de retrait WithdrawRequestNFT) | MIT | 13 | [lire](https://github.com/Crypt0-Gr0wth/etherfi-smart-contracts/tree/master) |
| [etherfi-protocol/weETH-cross-chain](https://github.com/etherfi-protocol/weETH-cross-chain) | Ether.fi weETH Cross-chain (lockboxes, messages et émission distante) | MIT | 4 | [lire](https://github.com/studiokvc/weeth-cross-chain/tree/master) |
| [FraxFinance/frxETH-public](https://github.com/FraxFinance/frxETH-public) | Frax Ether / frxETH (mint simple frxETH, coffre de rendement sfrxETH sur xERC4626, pile de validateurs OperatorRegistry) | GPL-2.0-or-later (contrats principaux) | 13 | [lire](https://github.com/Crypt0-Gr0wth/frxETH-public/tree/master) |
| [Layr-Labs/eigenlayer-contracts](https://github.com/Layr-Labs/eigenlayer-contracts) | EigenLayer | à vérifier | 6 | [lire](https://github.com/creativityventures/eigenlayer-contracts/tree/main) |
| [Layr-Labs/eigenlayer-middleware](https://github.com/Layr-Labs/eigenlayer-middleware) | EigenLayer Middleware | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/eigenlayer-middleware/tree/dev) |
| [lidofinance/core](https://github.com/lidofinance/core) | Lido (stETH rebasant a base de parts, staking router multi-modules, file de retraits, consensus d oracle) | GPL-3.0 | 18 | [lire](https://github.com/CryptoAstuce/core/tree/master) |
| [marinade-finance/liquid-staking-program](https://github.com/marinade-finance/liquid-staking-program) | Marinade liquid staking (délégation, mSOL, validators et unstake) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/liquid-staking-program/tree/main) |
| [PufferFinance/puffer-contracts](https://github.com/PufferFinance/puffer-contracts) | Puffer (pufETH, vault, tickets validateurs, retraits et oracle) | MIT | 5 | [lire](https://github.com/creativityventures/puffer-contracts/tree/master) |
| [rocket-pool/rocketpool](https://github.com/rocket-pool/rocketpool) | Rocket Pool (rETH a taux de change croissant, megapools multi-validateurs, bond d operateur, oracle DAO de confiance) | GPL-3.0-only | 13 | [lire](https://github.com/HereForTheTechNFT/rocketpool/tree/master) |
| [stakewise/v3-core](https://github.com/stakewise/v3-core) | StakeWise v3 (vaults de liquid staking permissionless, osToken surcollateralise, file de sortie, partage du MEV) | à vérifier | 13 | [lire](https://github.com/creativityventures/v3-core/tree/main) |
| [stakewise/v3-core](https://github.com/stakewise/v3-core) | StakeWise V3 (vaults, opérateurs, récompenses et retraits) | GPL-3.0 | 4 | [lire](https://github.com/cryptokvc/stakewise-v3-core/tree/main) |
| [symbioticfi/core](https://github.com/symbioticfi/core) | Symbiotic (collateral, vaults, opérateurs, réseaux, resolvers et slashing) | MIT | 4 | [lire](https://github.com/HereForTheTechNFT/symbiotic-core/tree/main) |

## Échanges : DEX, intents et market making

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [0xProject/0x-monorepo](https://github.com/0xProject/0x-monorepo) | 0x Protocol (ordres, asset proxies, settlement et outils développeur) | Apache-2.0 | 4 | [lire](https://github.com/HereForTheTechNFT/0x-monorepo/tree/development) |
| [0xProject/protocol](https://github.com/0xProject/protocol) | 0x Protocol | à vérifier | 6 | [lire](https://github.com/cryptokvc/protocol/tree/development) |
| [1inch/fusion-protocol](https://github.com/1inch/fusion-protocol) | 1inch Fusion (Dutch auctions, resolvers et exécution sans gas) | MIT | 4 | [lire](https://github.com/studiokvc/fusion-protocol/tree/master) |
| [1inch/limit-order-protocol](https://github.com/1inch/limit-order-protocol) | 1inch Limit Order Protocol (ordres limites, extensions, remplissage et annulation) | MIT | 6 | [lire](https://github.com/HereForTheTechNFT/limit-order-protocol/tree/master) |
| [ArrakisFinance/v2-core](https://github.com/ArrakisFinance/v2-core) | Arrakis V2 (vaults et gestion automatisée de liquidité) | MIT | 4 | [lire](https://github.com/studiokvc/arrakis-v2-core/tree/main) |
| [balancer/balancer-core](https://github.com/balancer/balancer-core) | Balancer v1 (pools multi-actifs a poids ponderes, swaps generalises, BPT) | GPL-3.0 | 13 | [lire](https://github.com/creativityventures/balancer-core/tree/master) |
| [balancer/balancer-v2-monorepo](https://github.com/balancer/balancer-v2-monorepo) | Balancer V2 (Vault, pools ponderes, swaps, liquidite, frais, flash loans) | GPL-3.0-or-later | 10 | [lire](https://github.com/studiokvc/balancer-v2-monorepo/tree/master) |
| [balancer/balancer-v3-monorepo](https://github.com/balancer/balancer-v3-monorepo) | Balancer V3 | à vérifier | 6 | [lire](https://github.com/A5Infinity/balancer-v3-monorepo/tree/main) |
| [cowprotocol/contracts](https://github.com/cowprotocol/contracts) | CoW Protocol (ordres signés, solvers, batch auctions et settlement) | GPL-3.0 | 4 | [lire](https://github.com/HereForTheTechNFT/cow-contracts/tree/main) |
| [cowprotocol/services](https://github.com/cowprotocol/services) | CoW Protocol | à vérifier | 11 | [lire](https://github.com/Crypt0-Gr0wth/services/tree/main) |
| [curvefi/curve-contract](https://github.com/curvefi/curve-contract) | Curve StableSwap (invariant hybride, pools de pret, metapools, ramping de A) | à vérifier | 18 | [lire](https://github.com/CryptoAstuce/curve-contract/tree/master) |
| [curvefi/curve-crypto-contract](https://github.com/curvefi/curve-crypto-contract) | Curve Crypto Contracts (invariant, pools, échanges et liquidité) | MIT | 4 | [lire](https://github.com/A5Infinity/curve-crypto-contract/tree/master) |
| [DODOEX/contractV2](https://github.com/DODOEX/contractV2) | DODO V2 (PMM, pools, liquidité proactive, routeurs et contrôles) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/contractV2/tree/main) |
| [Ellipsis-Labs/phoenix-v1](https://github.com/Ellipsis-Labs/phoenix-v1) | Phoenix Legacy (carnet d’ordres, priorités et règlement atomique) | MIT | 5 | [lire](https://github.com/DigitalA7/phoenix-v1/tree/master) |
| [GammaStrategies/hypervisor](https://github.com/GammaStrategies/hypervisor) | Gamma Hypervisor (liquidité concentrée et stratégies automatisées) | GPL-3.0 | 4 | [lire](https://github.com/studiokvc/gamma-hypervisor/tree/master) |
| [gnosis/zodiac](https://github.com/gnosis/zodiac) | Zodiac (avatars, modules, modifiers, guards et mastercopies) | LGPL-3.0+ | 5 | [lire](https://github.com/creativityventures/zodiac/tree/master) |
| [graphprotocol/contracts](https://github.com/graphprotocol/contracts) | The Graph Contracts | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/contracts/tree/main) |
| [graphprotocol/graph-node](https://github.com/graphprotocol/graph-node) | The Graph Node | à vérifier | 11 | [lire](https://github.com/DigitalA7/graph-node/tree/master) |
| [JulienKervarrec/challenge-scroll](https://github.com/JulienKervarrec/challenge-scroll) | Challenge Scroll (ERC-20, swap Uniswap V3, cotation, Permit2 et envoi de transaction) | MIT pour les fichiers Solidity consultés | 31 | [lire](https://github.com/JulienKervarrec/challenge-scroll/tree/main) |
| [jup-ag/jupiter-amm-implementation](https://github.com/jup-ag/jupiter-amm-implementation) | Jupiter AMM implementation (pools, swaps, liquidité et programmes Solana) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/jupiter-amm-implementation/tree/main) |
| [kleros/kleros-v2](https://github.com/kleros/kleros-v2) | Kleros v2 (juridictions, jurés, votes et appels) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/kleros-v2/tree/dev) |
| [lfj-gg/joe-v2](https://github.com/lfj-gg/joe-v2) | Liquidity Book / Trader Joe v2 (AMM a bins discrets, prix constant intra-bin, hooks programmables) | MIT | 13 | [lire](https://github.com/Crypt0-Gr0wth/joe-v2/tree/main) |
| [MeteoraAg/damm-v2](https://github.com/MeteoraAg/damm-v2) | Meteora DAMM V2 (pools, positions NFT, frais dynamiques, récompenses et verrouillage) | à vérifier | 6 | [lire](https://github.com/DigitalA7/damm-v2/tree/main) |
| [MeteoraAg/dlmm-sdk](https://github.com/MeteoraAg/dlmm-sdk) | Meteora DLMM SDK (bins, positions, swaps, ordres limites, frais et récompenses) | à vérifier | 5 | [lire](https://github.com/DigitalA7/dlmm-sdk/tree/main) |
| [MeteoraAg/stable-swap](https://github.com/MeteoraAg/stable-swap) | Saber StableSwap (invariant, pools, liquidité, swaps et clients) | Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/stable-swap/tree/master) |
| [openbook-dex/openbook-v2](https://github.com/openbook-dex/openbook-v2) | OpenBook V2 (ordres, lots, correspondance, événements et règlement) | AGPL-3.0 | 4 | [lire](https://github.com/JulienKervarrec/openbook-v2/tree/master) |
| [orca-so/whirlpools](https://github.com/orca-so/whirlpools) | Orca Whirlpools (liquidité concentrée, bins, swaps, positions et récompenses) | MIT | 6 | [lire](https://github.com/DigitalA7/whirlpools/tree/main) |
| [osmosis-labs/osmosis](https://github.com/osmosis-labs/osmosis) | Osmosis | à vérifier | 10 | [lire](https://github.com/studiokvc/osmosis/tree/main) |
| [paradigmxyz/reth](https://github.com/paradigmxyz/reth) | Reth (client d’exécution Rust, Engine API, crates modulaires, stockage, snapshots et performance) | Apache-2.0 + MIT | 8 | [lire](https://github.com/JulienKervarrec/reth-fr/tree/main) |
| [premiafinance/premia-contracts](https://github.com/premiafinance/premia-contracts) | Premia (options, pools, pricing, mining et vesting) | MIT et LGPL selon les fichiers | 4 | [lire](https://github.com/creativityventures/premia-contracts/tree/master) |
| [RamsesExchange/ramses-v3-contracts](https://github.com/RamsesExchange/ramses-v3-contracts) | Ramses V3 (pools concentrés, gauges, ticks et récompenses) | GPL-3.0 | 4 | [lire](https://github.com/studiokvc/ramses-v3-contracts/tree/main) |
| [raydium-io/raydium-clmm](https://github.com/raydium-io/raydium-clmm) | Raydium CLMM (ticks, positions, swaps, frais et récompenses) | Apache-2.0 | 4 | [lire](https://github.com/JulienKervarrec/raydium-clmm/tree/master) |
| [raydium-io/raydium-cp-swap](https://github.com/raydium-io/raydium-cp-swap) | Raydium CP-Swap (produit constant, liquidité, frais et Token-2022) | Apache-2.0 | 4 | [lire](https://github.com/JulienKervarrec/raydium-cp-swap/tree/master) |
| [RealityETH/reality-eth-monorepo](https://github.com/RealityETH/reality-eth-monorepo) | reality.eth (questions, réponses, bonds, contestations et indexation) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/reality-eth-monorepo/tree/main) |
| [solana-labs/solana-program-library](https://github.com/solana-labs/solana-program-library) | Solana Program Library | à vérifier | 11 | [lire](https://github.com/DigitalA7/solana-program-library/tree/master) |
| [streamr-dev/network-contracts](https://github.com/streamr-dev/network-contracts) | Streamr Network Contracts (contrats réseau, ABI, TypeChain, sous-graphes et adresses) | à vérifier | 5 | [lire](https://github.com/DigitalA7/network-contracts/tree/main) |
| [sushiswap/v2-core](https://github.com/sushiswap/v2-core) | SushiSwap V2 | à vérifier | 6 | [lire](https://github.com/cryptokvc/v2-core/tree/master) |
| [sushiswap/v3-core](https://github.com/sushiswap/v3-core) | SushiSwap V3 Core (liquidité concentrée, ticks et pools) | BUSL-1.1 / GPL-2.0-or-later | 4 | [lire](https://github.com/cryptokvc/v3-core/tree/master) |
| [Tokemak/tokemak-smart-contracts-public](https://github.com/Tokemak/tokemak-smart-contracts-public) | Tokemak (allocation de liquidité, stratégies et gouvernance) | MIT | 4 | [lire](https://github.com/studiokvc/tokemak-smart-contracts/tree/main) |
| [Uniswap/UniswapX](https://github.com/Uniswap/UniswapX) | UniswapX (ordres signés, reactors, fillers et règlement sans gas) | GPL-3.0 | 4 | [lire](https://github.com/studiokvc/UniswapX/tree/main) |
| [Uniswap/universal-router](https://github.com/Uniswap/universal-router) | Uniswap Universal Router (commandes, modules, swaps, paiements et chained actions) | BUSL-1.1 + MIT selon les fichiers | 5 | [lire](https://github.com/creativityventures/universal-router/tree/main) |
| [Uniswap/v2-core](https://github.com/Uniswap/v2-core) | Uniswap v2 (produit constant, flash swaps, oracle TWAP) | GPL-3.0 | 14 | [lire](https://github.com/JulienKervarrec/v2-core/tree/master) |
| [Uniswap/v3-core](https://github.com/Uniswap/v3-core) | Uniswap v3 (liquidite concentree, ticks, sqrtPriceX96, oracle TWAP, swaps flash) | à vérifier | 13 | [lire](https://github.com/HereForTheTechNFT/v3-core/tree/main) |
| [Uniswap/v3-periphery](https://github.com/Uniswap/v3-periphery) | Uniswap V3 Periphery | à vérifier | 6 | [lire](https://github.com/cryptokvc/v3-periphery/tree/main) |
| [Uniswap/v4-core](https://github.com/Uniswap/v4-core) | Uniswap v4 Core (singleton PoolManager, unlock, deltas, swaps, liquidite et hooks) | BUSL-1.1 + MIT selon les fichiers | 8 | [lire](https://github.com/JulienKervarrec/v4-core/tree/main) |
| [Uniswap/v4-core](https://github.com/Uniswap/v4-core) | Uniswap v4 Core (singleton PoolManager, deltas, hooks et règlement) | BUSL-1.1 et MIT selon les fichiers | 4 | [lire](https://github.com/artofbitcoin/v4-core/tree/main) |
| [Uniswap/v4-periphery](https://github.com/Uniswap/v4-periphery) | Uniswap v4 Periphery (positions NFT, actions, routeurs, swaps, deltas, quoter, StateView et hooks) | à vérifier | 8 | [lire](https://github.com/JulienKervarrec/v4-periphery-fr/tree/main) |
| [uniswapfoundation/v4-by-example](https://github.com/uniswapfoundation/v4-by-example) | Uniswap v4 (pools, hooks, swaps) | MIT | 7 | [lire](https://github.com/DigitalA7/v4-by-example/tree/gh-pages) |
| [velodrome-finance/contracts](https://github.com/velodrome-finance/contracts) | Velodrome V2 (AMM, veNFT, gauges et émissions) | MIT | 4 | [lire](https://github.com/studiokvc/velodrome-contracts/tree/main) |

## Dérivés, options et marchés prédictifs

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [AugurProject/augur](https://github.com/AugurProject/augur) | Augur (marchés prédictifs, reporting et règlement) | GPL-3.0 / MIT | 4 | [lire](https://github.com/cryptokvc/augur/tree/dev) |
| [derivexyz/v1-core](https://github.com/derivexyz/v1-core) | Lyra V1 (marchés d options, positions, prix, grecs, expiration, liquidité et couverture) | à vérifier | 5 | [lire](https://github.com/artofbitcoin/lyra-v1-core/tree/master) |
| [derivexyz/v1-core](https://github.com/derivexyz/v1-core) | Lyra V1 (marchés d’options, vaults, marge et liquidation) | MIT | 4 | [lire](https://github.com/cryptokvc/v1-core/tree/master) |
| [derivexyz/v2-core](https://github.com/derivexyz/v2-core) | Lyra V2 / Derive (options, positions, marges et liquidations) | MIT | 4 | [lire](https://github.com/A5Infinity/v2-core/tree/master) |
| [dolomite-exchange/dolomite-margin](https://github.com/dolomite-exchange/dolomite-margin) | Dolomite Margin (margin engine, accounts, markets, adapters et liquidations) | Apache-2.0 | 6 | [lire](https://github.com/HereForTheTechNFT/dolomite-margin/tree/v2) |
| [dydxprotocol/perpetual](https://github.com/dydxprotocol/perpetual) | dYdX Perpetual (marchés, marge, oracle et liquidation) | Apache-2.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/perpetual/tree/master) |
| [dydxprotocol/v4-chain](https://github.com/dydxprotocol/v4-chain) | dYdX Chain | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/v4-chain/tree/main) |
| [GainsNetwork/gTrade-v6.1](https://github.com/GainsNetwork/gTrade-v6.1) | Gains gTrade V6.1 (positions, marge, prix et liquidations) | MIT | 4 | [lire](https://github.com/studiokvc/gtrade-v6-1/tree/main) |
| [gmx-io/gmx-contracts](https://github.com/gmx-io/gmx-contracts) | GMX Contracts | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/gmx-contracts/tree/master) |
| [gnosis/conditional-tokens-contracts](https://github.com/gnosis/conditional-tokens-contracts) | Gnosis Conditional Tokens (conditions, collections et positions ERC-1155) | LGPL-3.0 | 4 | [lire](https://github.com/JulienKervarrec/conditional-tokens-contracts/tree/master) |
| [opynfinance/GammaProtocol](https://github.com/opynfinance/GammaProtocol) | Opyn Gamma | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/GammaProtocol/tree/master) |
| [Opynfinance/squeeth-monorepo](https://github.com/Opynfinance/squeeth-monorepo) | Squeeth (oSQTH, power perpetual, Crab, ZenBull et netting) | informations lues dans le dépôt amont | 4 | [lire](https://github.com/creativityventures/squeeth-monorepo/tree/main) |
| [overlay-market/v1-core](https://github.com/overlay-market/v1-core) | Overlay v1 Core (oracle, positions, garantie et liquidations) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/v1-core/tree/main) |
| [perpetual-protocol/perp-curie-contract](https://github.com/perpetual-protocol/perp-curie-contract) | Perpetual Protocol Curie (ClearingHouse, positions, funding, liquidation et Vault) | MIT | 5 | [lire](https://github.com/creativityventures/perp-curie-contract/tree/main) |
| [Polymarket/neg-risk-ctf-adapter](https://github.com/Polymarket/neg-risk-ctf-adapter) | Polymarket Neg Risk CTF Adapter (conditions, conversion, fusion et remboursement) | à vérifier | 4 | [lire](https://github.com/JulienKervarrec/neg-risk-ctf-adapter/tree/main) |
| [primitivefinance/v1-contracts](https://github.com/primitivefinance/v1-contracts) | Primitive V1 (options, positions et liquidité) | MIT | 4 | [lire](https://github.com/cryptokvc/v1-contracts/tree/develop) |
| [Synthetixio/synthetix-v3](https://github.com/Synthetixio/synthetix-v3) | Synthetix V3 | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/synthetix-v3/tree/main) |
| [Synthetixio/synthetix-v3](https://github.com/Synthetixio/synthetix-v3) | Synthetix V3 (router, marchés, positions et oracles) | MIT | 4 | [lire](https://github.com/cryptokvc/synthetix-v3/tree/main) |

## Vaults, rendement et gestion d'actifs

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [beefyfinance/beefy-contracts](https://github.com/beefyfinance/beefy-contracts) | Beefy Vaults (vaults, stratégies, récolte et frais) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/beefy-contracts/tree/master) |
| [convex-eth/platform](https://github.com/convex-eth/platform) | Convex | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/platform/tree/main) |
| [dexe-network/DeXe-Protocol](https://github.com/dexe-network/DeXe-Protocol) | DeXe Protocol (DAO, propositions, trésorerie, votes et gestionnaires) | MIT | 4 | [lire](https://github.com/HereForTheTechNFT/DeXe-Protocol/tree/master) |
| [enzymefinance/protocol](https://github.com/enzymefinance/protocol) | Enzyme Blue (fonds on-chain, modules et contrôles) | GPL-3.0 | 4 | [lire](https://github.com/cryptokvc/enzyme-protocol/tree/dev) |
| [Idle-Finance/idle-tranches](https://github.com/Idle-Finance/idle-tranches) | Idle Perpetual Yield Tranches (IdleCDO, tranches AA/BB, stratégies et récompenses) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/idle-tranches/tree/master) |
| [IndexCoop/index-protocol](https://github.com/IndexCoop/index-protocol) | Index Protocol (indices, pondération et rééquilibrage) | MIT | 4 | [lire](https://github.com/cryptokvc/index-protocol/tree/master) |
| [pendle-finance/pendle-core-v2-public](https://github.com/pendle-finance/pendle-core-v2-public) | Pendle Core V2 | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/pendle-core-v2-public/tree/main) |
| [ribbon-finance/ribbon-v2](https://github.com/ribbon-finance/ribbon-v2) | Ribbon V2 (vaults d options, rounds, pricing, settlement et gouvernance) | MIT | 4 | [lire](https://github.com/creativityventures/ribbon-v2/tree/master) |
| [solv-finance/solv-contracts-v3](https://github.com/solv-finance/solv-contracts-v3) | Solv V3 (SFT financiers, émission, marchés et remboursement) | MIT | 4 | [lire](https://github.com/A5Infinity/solv-contracts-v3/tree/main) |
| [yearn/yearn-vaults-v2](https://github.com/yearn/yearn-vaults-v2) | Yearn Vaults V2 (vaults, stratégies, debt ratios, harvest et yShares) | AGPL-3.0 | 6 | [lire](https://github.com/HereForTheTechNFT/yearn-vaults-v2/tree/master) |
| [yearn/yearn-vaults-v2](https://github.com/yearn/yearn-vaults-v2) | Yearn Vaults v2 (coffres, parts, stratégies, rapports, frais et arrêt d’urgence) | AGPL-3.0 | 5 | [lire](https://github.com/creativityventures/yearn-vaults-v2/tree/master) |
| [yearn/yearn-vaults-v3](https://github.com/yearn/yearn-vaults-v3) | Yearn Vaults V3 (parts, stratégies, rapports, profits et frais) | AGPL-3.0 | 4 | [lire](https://github.com/JulienKervarrec/yearn-vaults-v3/tree/master) |

## Bridges et interopérabilité

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [across-protocol/contracts](https://github.com/across-protocol/contracts) | Across Protocol (bridge par intents et relayeurs, SpokePool/HubPool, racines merkle bondees, oracle optimiste UMA) | BUSL-1.1 | 13 | [lire](https://github.com/Crypt0-Gr0wth/across-contracts/tree/master) |
| [across-protocol/contracts](https://github.com/across-protocol/contracts) | Across Protocol (HubPool, SpokePool, dépôts, remplissage, lots Merkle et règlement) | BUSL-1.1 | 5 | [lire](https://github.com/artofbitcoin/across-contracts/tree/master) |
| [axelarnetwork/axelar-core](https://github.com/axelarnetwork/axelar-core) | Axelar Core (consensus, multisig, gateway et appels inter-chaînes) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/axelar-core/tree/main) |
| [axelarnetwork/axelar-gmp-sdk-solidity](https://github.com/axelarnetwork/axelar-gmp-sdk-solidity) | Axelar GMP SDK (gateways, messages, preuves, tokens, express et gouvernance) | MIT | 5 | [lire](https://github.com/creativityventures/axelar-gmp-sdk-solidity/tree/main) |
| [connext/monorepo](https://github.com/connext/monorepo) | Connext (xcall, routeurs, liquidité, transport, vérification et relai) | MIT | 6 | [lire](https://github.com/creativityventures/monorepo/tree/main) |
| [cosmos/ibc-go](https://github.com/cosmos/ibc-go) | Cosmos IBC | à vérifier | 7 | [lire](https://github.com/studiokvc/ibc-go/tree/main) |
| [dev-bootcamp/study-bridge](https://github.com/dev-bootcamp/study-bridge) | Bridge burn/mint avec signature de validateur | MIT | 7 | [lire](https://github.com/DigitalA7/study-bridge/tree/master) |
| [ethereum-optimism/optimism](https://github.com/ethereum-optimism/optimism) | Optimism | MIT | 6 | [lire](https://github.com/HereForTheTechNFT/optimism/tree/develop) |
| [hop-protocol/contracts](https://github.com/hop-protocol/contracts) | Hop Protocol (hTokens, AMM, bonders, TransferRoots et challenges) | MIT | 4 | [lire](https://github.com/HereForTheTechNFT/contracts/tree/master) |
| [hop-protocol/hop](https://github.com/hop-protocol/hop) | Hop Protocol (bridge L1/L2, bonder, liquidite, AMM, preuves de retrait, SDK et watchers) | MIT | 8 | [lire](https://github.com/JulienKervarrec/hop/tree/develop) |
| [hyperlane-xyz/hyperlane-monorepo](https://github.com/hyperlane-xyz/hyperlane-monorepo) | Hyperlane | à vérifier | 6 | [lire](https://github.com/A5Infinity/hyperlane-monorepo/tree/main) |
| [LayerZero-Labs/LayerZero-v2](https://github.com/LayerZero-Labs/LayerZero-v2) | LayerZero V2 | à vérifier | 6 | [lire](https://github.com/cryptokvc/LayerZero-v2/tree/main) |
| [smartcontractkit/chainlink-ccip](https://github.com/smartcontractkit/chainlink-ccip) | Chainlink CCIP | à vérifier | 11 | [lire](https://github.com/DigitalA7/chainlink-ccip/tree/main) |
| [stargate-protocol/stargate](https://github.com/stargate-protocol/stargate) | Stargate (bridge, pools, liquidité unifiée et messages cross-chain) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/stargate/tree/main) |
| [wormhole-foundation/wormhole](https://github.com/wormhole-foundation/wormhole) | Wormhole | à vérifier | 6 | [lire](https://github.com/A5Infinity/wormhole/tree/main) |

## Comptes, wallets et identité

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [argentlabs/argent-contracts](https://github.com/argentlabs/argent-contracts) | Argent Wallet (wallet contractuel, guardians, récupération et modules) | GPL-3.0 | 4 | [lire](https://github.com/A5Infinity/argent-contracts/tree/develop) |
| [eth-infinitism/account-abstraction](https://github.com/eth-infinitism/account-abstraction) | ERC-4337 (EntryPoint, UserOperation, paymasters, EIP-7702) | à vérifier | 14 | [lire](https://github.com/JulienKervarrec/account-abstraction/tree/develop) |
| [farcasterxyz/contracts](https://github.com/farcasterxyz/contracts) | Farcaster Contracts (IdRegistry, KeyRegistry, stockage, récupération et gateways) | MIT | 5 | [lire](https://github.com/creativityventures/contracts/tree/main) |
| [Instadapp/avocado-contracts-public](https://github.com/Instadapp/avocado-contracts-public) | Avocado (proxies, multisig, signatures EIP-712, forwarder et registry) | MIT | 4 | [lire](https://github.com/A5Infinity/avocado-contracts-public/tree/main) |
| [Instadapp/dsa-contracts](https://github.com/Instadapp/dsa-contracts) | Instadapp DSA | à vérifier | 6 | [lire](https://github.com/cryptokvc/dsa-contracts/tree/master) |
| [Instadapp/dsa-contracts](https://github.com/Instadapp/dsa-contracts) | Instadapp DSA (smart accounts, connecteurs, composition et permissions) | à vérifier | 8 | [lire](https://github.com/artofbitcoin/dsa-contracts/tree/master) |
| [lens-protocol/core](https://github.com/lens-protocol/core) | Lens Protocol | à vérifier | 6 | [lire](https://github.com/HereForTheTechNFT/core/tree/master) |
| [reown-com/appkit](https://github.com/reown-com/appkit) | Reown AppKit (onboarding, authentification, multi-chaînes, swaps, sponsoring et SDK) | Reown AppKit Community License | 5 | [lire](https://github.com/DigitalA7/appkit/tree/main) |
| [safe-fndn/safe-smart-account](https://github.com/safe-fndn/safe-smart-account) | Safe Smart Account | LGPL-3.0 | 6 | [lire](https://github.com/creativityventures/safe-smart-account/tree/main) |
| [safe-global/safe-smart-account](https://github.com/safe-global/safe-smart-account) | Safe Smart Account | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/safe-smart-account/tree/main) |
| [WalletConnect/walletconnect-monorepo](https://github.com/WalletConnect/walletconnect-monorepo) | WalletConnect Monorepo v2 (sessions, packages, providers et demandes de signature) | WalletConnect Community License | 5 | [lire](https://github.com/DigitalA7/walletconnect-monorepo/tree/v2.0) |

## Oracles, paiements et automatisation

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [api3dao/contracts](https://github.com/api3dao/contracts) | API3 (dAPI, proxies, abonnements et OEV) | MIT | 4 | [lire](https://github.com/studiokvc/api3-contracts/tree/main) |
| [ethereum-push-notification-service/push-smart-contracts](https://github.com/ethereum-push-notification-service/push-smart-contracts) | Push Smart Contracts (canaux, abonnements, permissions et délégation) | MIT | 4 | [lire](https://github.com/A5Infinity/push-notifications-smart-contracts/tree/master) |
| [gelatodigital/automate](https://github.com/gelatodigital/automate) | Gelato Automate (tâches, financement, resolvers, exécution et permissions) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/automate/tree/master) |
| [keep3r-network/keep3r.network](https://github.com/keep3r-network/keep3r.network) | Keep3r Network (keepers, jobs, bonding et récompenses) | MIT | 4 | [lire](https://github.com/cryptokvc/keep3r.network/tree/master) |
| [PoolTogether/v5-twab-controller](https://github.com/PoolTogether/v5-twab-controller) | PoolTogether TWAB Controller (observations, moyennes temporelles et récompenses) | MIT | 4 | [lire](https://github.com/Crypt0-Gr0wth/v5-twab-controller/tree/main) |
| [pyth-network/pyth-crosschain](https://github.com/pyth-network/pyth-crosschain) | Pyth Crosschain (Pythnet, Hermes, prix et mises à jour) | Apache-2.0 | 4 | [lire](https://github.com/studiokvc/pyth-crosschain/tree/main) |
| [redstone-finance/redstone-oracles-monorepo](https://github.com/redstone-finance/redstone-oracles-monorepo) | RedStone (payloads transactionnels, signataires et connecteurs EVM) | BUSL-1.1 | 4 | [lire](https://github.com/studiokvc/redstone-oracles/tree/main) |
| [sablier-labs/v2-core](https://github.com/sablier-labs/v2-core) | Sablier V2 (streams, retraits, modèles linéaires et cliffs) | GPL-3.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/evm-monorepo/tree/main) |
| [smartcontractkit/chainlink](https://github.com/smartcontractkit/chainlink) | Chainlink Contracts | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/chainlink/tree/develop) |
| [stellar/stellar-core](https://github.com/stellar/stellar-core) | Stellar Core | à vérifier | 8 | [lire](https://github.com/studiokvc/stellar-core/tree/master) |
| [superfluid-finance/protocol-monorepo](https://github.com/superfluid-finance/protocol-monorepo) | Superfluid (flux CFA, distributions GDA, solvabilité et callbacks) | AGPL-3.0 | 4 | [lire](https://github.com/Crypt0-Gr0wth/protocol-monorepo/tree/dev) |
| [superfluid-org/protocol-monorepo](https://github.com/superfluid-org/protocol-monorepo) | Superfluid (Host, CFA/IDA, Super Tokens, callbacks et solvabilité) | AGPL-3.0 | 6 | [lire](https://github.com/HereForTheTechNFT/protocol-monorepo/tree/dev) |
| [UMAprotocol/optimistic-oracle-dapp-v2](https://github.com/UMAprotocol/optimistic-oracle-dapp-v2) | UMA Optimistic Oracle DApp v2 (assertions, bonds, contestations et règlement) | MIT | 4 | [lire](https://github.com/A5Infinity/optimistic-oracle-dapp-v2/tree/master) |
| [UMAprotocol/protocol](https://github.com/UMAprotocol/protocol) | UMA Protocol (assertions, bonds, disputes, DVM, Finder, Skinny Oracle, SDK et bots) | AGPL-3.0 | 8 | [lire](https://github.com/JulienKervarrec/uma-protocol/tree/master) |
| [Uniswap/permit2](https://github.com/Uniswap/permit2) | Permit2 | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/permit2/tree/main) |
| [x402-foundation/x402](https://github.com/x402-foundation/x402) | x402 (protocole de paiement sur HTTP 402) | Apache-2.0 | 6 | [lire](https://github.com/DigitalA7/x402/tree/main) |

## DAO et gouvernance

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [daohaus/daohaus-contracts](https://github.com/daohaus/daohaus-contracts) | DAOhaus contracts (hubs, proposals, shares, ressources et exécution) | MIT | 5 | [lire](https://github.com/creativityventures/daohaus-contracts/tree/master) |
| [JoinColony/colonyNetwork](https://github.com/JoinColony/colonyNetwork) | Colony Network (organisations, réputation, domaines et Funding Pots) | GPL-3.0 | 4 | [lire](https://github.com/A5Infinity/colonyNetwork/tree/develop) |
| [PartyDAO/party-protocol](https://github.com/PartyDAO/party-protocol) | Party Protocol (groupes, propositions, votes et distributions) | MIT | 4 | [lire](https://github.com/A5Infinity/party-protocol/tree/main) |

## Ethereum, rollups et infrastructure

| Projet étudié | Sujet | Licence du code | Chapitres | Parcours |
|---|---|---|---|---|
| [a16z/helios](https://github.com/a16z/helios) | Helios (client léger multichaîne, preuves eth_getProof, checkpoints, Ethereum, OP Stack et Linea) | MIT | 8 | [lire](https://github.com/JulienKervarrec/helios-fr/tree/master) |
| [algorandfoundation/algokit-utils-ts](https://github.com/algorandfoundation/algokit-utils-ts) | AlgoKit Utils TypeScript (client Algorand, transactions, contrats, configuration et migrations) | MIT | 5 | [lire](https://github.com/DigitalA7/algokit-utils-ts/tree/main) |
| [alloy-rs/alloy](https://github.com/alloy-rs/alloy) | Alloy (primitives Ethereum, providers RPC, reseaux, transactions, signers et bindings Solidity) | MIT / Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/alloy/tree/main) |
| [aptos-labs/aptos-core](https://github.com/aptos-labs/aptos-core) | Aptos Core (Move, exécution, consensus, réseau, stockage et SDK) | Innovation-Enabling Source Code License | 5 | [lire](https://github.com/DigitalA7/aptos-core/tree/main) |
| [argotorg/solidity](https://github.com/argotorg/solidity) | Solidity (compilateur, ABI, types, IR, optimisations et securite des smart contracts) | GPL-3.0 / MIT selon les composants | 6 | [lire](https://github.com/CryptoAstuce/solidity/tree/develop) |
| [ArweaveTeam/arweave](https://github.com/ArweaveTeam/arweave) | Arweave | GPL-2.0 | 9 | [lire](https://github.com/studiokvc/arweave/tree/master) |
| [ava-labs/avalanchego](https://github.com/ava-labs/avalanchego) | AvalancheGo | à vérifier | 8 | [lire](https://github.com/studiokvc/avalanchego/tree/master) |
| [base/benchmark](https://github.com/base/benchmark) | Base Benchmark | à vérifier | 8 | [lire](https://github.com/A5Infinity/benchmark/tree/main) |
| [base/nitro-validator](https://github.com/base/nitro-validator) | Base Nitro Validator | à vérifier | 7 | [lire](https://github.com/A5Infinity/nitro-validator/tree/main) |
| [bluealloy/revm](https://github.com/bluealloy/revm) | revm (moteur EVM Rust, contexte, transactions, precompiles et inspection) | MIT / Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/revm/tree/main) |
| [celestiaorg/celestia-app](https://github.com/celestiaorg/celestia-app) | Celestia App | à vérifier | 10 | [lire](https://github.com/studiokvc/celestia-app/tree/main) |
| [cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk) | Cosmos SDK | à vérifier | 11 | [lire](https://github.com/DigitalA7/cosmos-sdk/tree/main) |
| [ENSdomains/ens-contracts](https://github.com/ENSdomains/ens-contracts) | ENS | à vérifier | 6 | [lire](https://github.com/cryptokvc/ens-contracts/tree/staging) |
| [ethereum-attestation-service/eas-contracts](https://github.com/ethereum-attestation-service/eas-contracts) | Ethereum Attestation Service (schemas, attestations, revocation, resolvers, delegation EIP-712 et indexation) | MIT | 8 | [lire](https://github.com/JulienKervarrec/eas-contracts/tree/master) |
| [ethereum/consensus-specs](https://github.com/ethereum/consensus-specs) | Ethereum Consensus Specs | CC-BY-4.0 | 6 | [lire](https://github.com/HereForTheTechNFT/consensus-specs/tree/master) |
| [ethereum/execution-apis](https://github.com/ethereum/execution-apis) | Ethereum Execution APIs (JSON-RPC, eth/engine, payloads, transaction pool, schemas et erreurs) | CC0-1.0 | 6 | [lire](https://github.com/CryptoAstuce/execution-apis/tree/main) |
| [ethereum/portal-network-specs](https://github.com/ethereum/portal-network-specs) | Portal Network (Discv5, History, State, content keys, routage, wire protocol et JSON-RPC) | CC0-1.0 | 6 | [lire](https://github.com/CryptoAstuce/portal-network-specs/tree/master) |
| [ethereum/remix-desktop](https://github.com/ethereum/remix-desktop) | Remix Desktop (Electron, IDE embarque, fichiers locaux, IPC, packaging et securite) | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/remix-desktop/tree/master) |
| [ethereumjs/ethereumjs-monorepo](https://github.com/ethereumjs/ethereumjs-monorepo) | EthereumJS (EVM, transactions, blocs, etat, MPT, hardforks et packages TypeScript) | MPL-2.0 selon les packages | 8 | [lire](https://github.com/JulienKervarrec/ethereumjs-fr/tree/master) |
| [filecoin-project/lotus](https://github.com/filecoin-project/lotus) | Filecoin Lotus | à vérifier | 9 | [lire](https://github.com/studiokvc/lotus/tree/master) |
| [flashbots/mev-boost](https://github.com/flashbots/mev-boost) | Flashbots MEV-Boost | à vérifier | 6 | [lire](https://github.com/CryptoAstuce/mev-boost/tree/develop) |
| [foundry-rs/foundry](https://github.com/foundry-rs/foundry) | Foundry (Forge, Cast, Anvil, Chisel et Forge LSP) | Apache-2.0 + MIT | 5 | [lire](https://github.com/JulienKervarrec/foundry-fr/tree/master) |
| [ipfs/kubo](https://github.com/ipfs/kubo) | IPFS Kubo | à vérifier | 11 | [lire](https://github.com/DigitalA7/kubo/tree/master) |
| [jito-foundation/jito-solana](https://github.com/jito-foundation/jito-solana) | Jito Solana (block engine, bundles, relais et validation) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/jito-solana/tree/master) |
| [livepeer/protocol](https://github.com/livepeer/protocol) | Livepeer (bonding, délégation, workers, inflation et tickets de paiement) | à vérifier | 4 | [lire](https://github.com/artofbitcoin/protocol/tree/delta) |
| [matter-labs/era-system-contracts](https://github.com/matter-labs/era-system-contracts) | zkSync Era System Contracts (bootloader, déploiement et messagerie L1/L2) | MIT | 4 | [lire](https://github.com/studiokvc/era-system-contracts/tree/main) |
| [MeteoraAg/dynamic-bonding-curve](https://github.com/MeteoraAg/dynamic-bonding-curve) | Meteora Dynamic Bonding Curve (courbes, frais, graduation et migration) | à vérifier | 6 | [lire](https://github.com/DigitalA7/dynamic-bonding-curve/tree/main) |
| [near/nearcore](https://github.com/near/nearcore) | NEAR Core (client de référence, runtime, réseau, état, SDK et validation) | Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/nearcore/tree/master) |
| [NethermindEth/nethermind](https://github.com/NethermindEth/nethermind) | Nethermind (client .NET, Snap Sync, EVM, etat, JSON-RPC, plugins, monitoring et execution stateless) | LGPL-3.0 | 6 | [lire](https://github.com/CryptoAstuce/nethermind/tree/master) |
| [OffchainLabs/nitro](https://github.com/OffchainLabs/nitro) | Arbitrum Nitro | à vérifier | 6 | [lire](https://github.com/JulienKervarrec/nitro/tree/master) |
| [OpenZeppelin/openzeppelin-contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) | Tokens OpenZeppelin (ERC-20, ERC-721, ERC-1155, wrappers, ERC-4626, signatures, gouvernance, ERC-2981, ERC-6909) | MIT | 14 | [lire](https://github.com/DigitalA7/openzeppelin-contracts/tree/master) |
| [paritytech/polkadot-sdk](https://github.com/paritytech/polkadot-sdk) | Polkadot SDK | à vérifier | 11 | [lire](https://github.com/DigitalA7/polkadot-sdk/tree/master) |
| [paritytech/substrate](https://github.com/paritytech/substrate) | Substrate | à vérifier | 11 | [lire](https://github.com/DigitalA7/substrate/tree/master) |
| [remix-project-org/remix-project](https://github.com/remix-project-org/remix-project) | Remix Project (IDE, compilation Solidity, AST, plugins, bibliotheques et debogage) | Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/remix-project/tree/master) |
| [sigp/lighthouse](https://github.com/sigp/lighthouse) | Lighthouse (Beacon Chain, synchronisation, attestations, fork choice, finalite et slashing) | Apache-2.0 | 6 | [lire](https://github.com/CryptoAstuce/lighthouse/tree/stable) |
| [status-im/nimbus-eth2](https://github.com/status-im/nimbus-eth2) | Nimbus (Beacon Chain, etat consensus, synchronisation, attestations, fork choice et finalite) | Apache-2.0 / MIT selon les composants | 6 | [lire](https://github.com/CryptoAstuce/nimbus-eth2/tree/stable) |
| [thirdweb-dev/contracts](https://github.com/thirdweb-dev/contracts) | thirdweb Contracts (contrats préconstruits, extensions, composition, audits et déploiement) | Apache-2.0 | 5 | [lire](https://github.com/DigitalA7/thirdweb-contracts/tree/main) |
| [transmissions11/solmate](https://github.com/transmissions11/solmate) | Solmate (briques Solidity gas-optimisees : ERC20, ERC721, ERC4626, permit EIP-2612, Auth/Owned, SafeTransferLib) | AGPL-3.0-only | 13 | [lire](https://github.com/creativityventures/solmate/tree/main) |
| [Vectorized/dn404](https://github.com/Vectorized/dn404) | DN404 | à vérifier | 6 | [lire](https://github.com/A5Infinity/dn404/tree/main) |
| [Vectorized/solady](https://github.com/Vectorized/solady) | Solady | à vérifier | 6 | [lire](https://github.com/A5Infinity/solady/tree/main) |

## Licence

Le texte de ce dépôt est publié sous licence [CC BY 4.0](LICENSE). Chaque parcours lié reste soumis à la licence de son dépôt, et le code qu'il cite à la licence de son projet d'origine.
