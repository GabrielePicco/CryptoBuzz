---
layout: post
title:  "Algorand will upgrade in a month: 6x TPS, state proofs, AVM v7 (on chain randomness and more)"
description: "IMPORTANT  This release requires a protocol upgrade.  This release contains a consensus protocol upgrade, which implements the following spec: https://github.com/algorandfoundation/specs/tree/2dd5435993f6f6d65691140f592ebca5ef19ffbd



What's New

State Proofs: lightweight, cryptographically provable, portable proofs of Algorand state that let dapps on other blockchains trustlessly verify Algorand transactions, making it safer and easier to develop and use cross-chain products and services.
Max TPS of 6k

Larger blocks: ~5x increase in max-block size (from 1MB to 5MiB), allowing up to ~25k transactions per block.
Shorter round times: ~0.5s reduction in average round times (approaching ~3.9s).


AVM v7

On-chain randomness beacons and oracles can now be built by taking advantage of the new block and vrf_verify opcodes.
Unfunded accounts (with 0 microalgo) can now issue transactions as long as their fees are covered by fee pooling in the transaction group.
App calls are now implicitly given access to the app accounts for the apps specified in the foreign apps array.



Changelog
New Features

Algod: State Proofs (#4226)
AVM: randomness support (#3900)
AVM: Refactor Pseudo-ops (#4170)
AVM: Provide access to large programs in a txn, for read and inner submit (#4148)
Goal Network Catchup: automatically fetch catchpoint if not provided (#4012)

Enhancements

320 Rounds: Add logging for new logic (#4332)
AVM: Spec updates for v7 (#4347)
AVM: Fix crypto benchmarks from bitrot (#4340)
AVM: Move elliptic curve math up to v8 so it doesn't get released (#4282)
AVM: Consolidate TEAL and AVM versioning (#4269)
AVM: Don't parallelize tests that use shared for loop var (#4253)
Algod: rename some API operations for clarity (#4376)
Ci: Run go vet on the entire repo (#4312)
Ci: Add parameter to run Nightly Test (#4299)
Cicd: add mac arm64 to integration tests (#4167)
Cicd: upgrade xcode on circleci macos executors (#4188)
Cicd: remove unused genesis in stash (#4155)
Config: set MaxAcctLookback to 4 (#4296)
Config: update vFuture consensus and configuration for 5MB blocks (#4273)
Consensus: introduce v33, v34 (#4334)
Crypto: remove batch verification flag (#3781)
Docs: Control the specs generated seperately from logic.LogicVersion (#4361)
Enhancement: Detect when valid partkeys represent an offline or closed account (#4030)
Github-actions: add Not-Yet-Enabled and Skip-Release-Notes labels (#4196)
Goal: Allow --signer to send txns from rekeyed accounts (#4175)
Goal: Make the -n flag (network name) optional. Get it from template file (#4159)
Ledger: restore pointer receivers and args from #4003 (#4239)
Ledger: shorter deltas lookback implementation (320 rounds project) (#4003)
Loadgenerator: add multiple accounts config option (#4321)
Logging: Add a way to inject an external logger. (#4158)
Metrics: Don't allocate when invoking the Inc() fastpath (#4193)
Network: make txBacklogSize responsive to block size (#4377)
Optimization: Use bits package for Muldiv. 266x speedup (#4210)
Tests: extended logging on expect test abort (#4343)
Tests: cluster scenarios for 2022-07 (#4331)
Tests: touch fields_string.go so everything is rebuilt in codegen verification (#4330)
Tests: Make e2e subs report individual results better (#4286)
Tests: Fix typo in ledger_test.go (#4297)
Tests: Support multiple e2e test archives. (#4284)
Tests: Fail codegen_verification if dump_genesis.sh is bad (#4277)
Tests: use T.TempDir to create temporary test directory (#4256)
Tests: fixes to catchpoint e2e tests (#4236)
Tests: pingpong fixes and heap watch reporting (#4069)
Tools: adapt loadgenerator to cluster testing (#4324)
Tools: Fixing updater to accept m1 (Darwin arm64) (#4099)

Bugfixes

AVM: Make txn FirstValidTime and block opcode available in logicsigs (#4371)
Algod: fix issues causing database is locked sqlite error (#4110)
Bug Fix: Adds ephemeral Flag and Better Error messages (#4245)
Catchpointdump: fix downloading logic (#4171)
Goal: Fix source map mappings key and use relative line values (#4198)
Ledger: fix accountsMu usage (#4280)
Ledger: remove txtail from data race test (#4315)
Tests: fix TestAccountsCanSendMoney #3 (#4379)
Tests: un-shadow loadgen privateKeys var (#4380)
Tests: fix TestAssetValidRounds (#4351)
Tests: fix TestAccountsCanSendMoney #2 (#4374)
Tests: fix TestAccountsCanSendMoney (#4354)
Tests: close ledger after TestCatchupUnmatchedCertificate (#4348)
Tests: simplify TestWebsocketNetworkMessageOfInterest (#4341)
Tests: pass fixture by pointer instead of by value, since it contains a mutex (#4310)
Tests: fix TestParticipationDB_Locking (#4265)
Tools: goal logging send fixes (#4281)
Txns: Allow \"empty\" accounts to be Senders if someone else pays (#4151)

Activations (previously in vFuture)

AVM: Add bn256 pairing opcodes experimentally (#4013)
AVM: base64_decode can decode padded or unpadded encodings (#4015)
AVM: Allow immutable access to foreign app accounts (#3994)
AVM: Unify inner transaction ID calculation (#3927)
AVM: replace opcodes (#4129)
AVM: Set proper costs for json_ref (#4096)
StateProofs: New block header field - SHA256 merkle root of the transactions (#3829)
StateProofs: fix GetProof endpoint response (#3985)

Additional Resources

Algorand Forum
Developer Documentation"
date: "2022-08-11 23:11:04"
categories: ['4383', 'algodevopsservice', 'request']
score: 193
image: "https://i.imgur.com/kf6YLR4.jpg"
tags: ['4383', 'algodevopsservice', 'request']
link: "https://github.com/algorand/go-algorand/pull/4383"
---

IMPORTANT  This release requires a protocol upgrade.  This release contains a consensus protocol upgrade, which implements the following spec: https://github.com/algorandfoundation/specs/tree/2dd5435993f6f6d65691140f592ebca5ef19ffbd



What's New

State Proofs: lightweight, cryptographically provable, portable proofs of Algorand state that let dapps on other blockchains trustlessly verify Algorand transactions, making it safer and easier to develop and use cross-chain products and services.
Max TPS of 6k

Larger blocks: ~5x increase in max-block size (from 1MB to 5MiB), allowing up to ~25k transactions per block.
Shorter round times: ~0.5s reduction in average round times (approaching ~3.9s).


AVM v7

On-chain randomness beacons and oracles can now be built by taking advantage of the new block and vrf_verify opcodes.
Unfunded accounts (with 0 microalgo) can now issue transactions as long as their fees are covered by fee pooling in the transaction group.
App calls are now implicitly given access to the app accounts for the apps specified in the foreign apps array.



Changelog
New Features

Algod: State Proofs (#4226)
AVM: randomness support (#3900)
AVM: Refactor Pseudo-ops (#4170)
AVM: Provide access to large programs in a txn, for read and inner submit (#4148)
Goal Network Catchup: automatically fetch catchpoint if not provided (#4012)

Enhancements

320 Rounds: Add logging for new logic (#4332)
AVM: Spec updates for v7 (#4347)
AVM: Fix crypto benchmarks from bitrot (#4340)
AVM: Move elliptic curve math up to v8 so it doesn't get released (#4282)
AVM: Consolidate TEAL and AVM versioning (#4269)
AVM: Don't parallelize tests that use shared for loop var (#4253)
Algod: rename some API operations for clarity (#4376)
Ci: Run go vet on the entire repo (#4312)
Ci: Add parameter to run Nightly Test (#4299)
Cicd: add mac arm64 to integration tests (#4167)
Cicd: upgrade xcode on circleci macos executors (#4188)
Cicd: remove unused genesis in stash (#4155)
Config: set MaxAcctLookback to 4 (#4296)
Config: update vFuture consensus and configuration for 5MB blocks (#4273)
Consensus: introduce v33, v34 (#4334)
Crypto: remove batch verification flag (#3781)
Docs: Control the specs generated seperately from logic.LogicVersion (#4361)
Enhancement: Detect when valid partkeys represent an offline or closed account (#4030)
Github-actions: add Not-Yet-Enabled and Skip-Release-Notes labels (#4196)
Goal: Allow --signer to send txns from rekeyed accounts (#4175)
Goal: Make the -n flag (network name) optional. Get it from template file (#4159)
Ledger: restore pointer receivers and args from #4003 (#4239)
Ledger: shorter deltas lookback implementation (320 rounds project) (#4003)
Loadgenerator: add multiple accounts config option (#4321)
Logging: Add a way to inject an external logger. (#4158)
Metrics: Don't allocate when invoking the Inc() fastpath (#4193)
Network: make txBacklogSize responsive to block size (#4377)
Optimization: Use bits package for Muldiv. 266x speedup (#4210)
Tests: extended logging on expect test abort (#4343)
Tests: cluster scenarios for 2022-07 (#4331)
Tests: touch fields_string.go so everything is rebuilt in codegen verification (#4330)
Tests: Make e2e subs report individual results better (#4286)
Tests: Fix typo in ledger_test.go (#4297)
Tests: Support multiple e2e test archives. (#4284)
Tests: Fail codegen_verification if dump_genesis.sh is bad (#4277)
Tests: use T.TempDir to create temporary test directory (#4256)
Tests: fixes to catchpoint e2e tests (#4236)
Tests: pingpong fixes and heap watch reporting (#4069)
Tools: adapt loadgenerator to cluster testing (#4324)
Tools: Fixing updater to accept m1 (Darwin arm64) (#4099)

Bugfixes

AVM: Make txn FirstValidTime and block opcode available in logicsigs (#4371)
Algod: fix issues causing database is locked sqlite error (#4110)
Bug Fix: Adds ephemeral Flag and Better Error messages (#4245)
Catchpointdump: fix downloading logic (#4171)
Goal: Fix source map mappings key and use relative line values (#4198)
Ledger: fix accountsMu usage (#4280)
Ledger: remove txtail from data race test (#4315)
Tests: fix TestAccountsCanSendMoney #3 (#4379)
Tests: un-shadow loadgen privateKeys var (#4380)
Tests: fix TestAssetValidRounds (#4351)
Tests: fix TestAccountsCanSendMoney #2 (#4374)
Tests: fix TestAccountsCanSendMoney (#4354)
Tests: close ledger after TestCatchupUnmatchedCertificate (#4348)
Tests: simplify TestWebsocketNetworkMessageOfInterest (#4341)
Tests: pass fixture by pointer instead of by value, since it contains a mutex (#4310)
Tests: fix TestParticipationDB_Locking (#4265)
Tools: goal logging send fixes (#4281)
Txns: Allow \"empty\" accounts to be Senders if someone else pays (#4151)

Activations (previously in vFuture)

AVM: Add bn256 pairing opcodes experimentally (#4013)
AVM: base64_decode can decode padded or unpadded encodings (#4015)
AVM: Allow immutable access to foreign app accounts (#3994)
AVM: Unify inner transaction ID calculation (#3927)
AVM: replace opcodes (#4129)
AVM: Set proper costs for json_ref (#4096)
StateProofs: New block header field - SHA256 merkle root of the transactions (#3829)
StateProofs: fix GetProof endpoint response (#3985)

Additional Resources

Algorand Forum
Developer Documentation

## Highlights

- This release requires a consensus protocol upgrade.
- State Proofs are lightweight, cryptographically provable, portable proofs of Algorand state that let dapps on other blockchains trustlessly verify transactions.
- Unfunded accounts (with 0 microalgo) can now issue transactions as long as their fees are covered by fee pooling in the transaction group.
- Shorter round times: ~0.5s reduction in average round times (approaching ~3.9s) On-chain randomness beacons and oracles can now be built by taking advantage of the new block and vrf_verify opcodes.
- New rules: Don't parallelize tests that use shared for loop var (#4253)

---
