# Salty.IO - Mitigation Review details
- Total Prize Pool: $25,000 in USDC 
- [Warden guidelines for C4 mitigation reviews](https://code4rena.notion.site/Guidelines-for-C4-mitigation-reviews-ed10fc5cfbf640bd8dcec66f38b343c4)
- Submit findings [using the C4 form](https://code4rena.com/contests/2024-03-saltyio-mitigation-review/submit)
- Starts March 1, 20:00 UTC
- Ends March 8, 20:00 UTC

## Important note 

Each warden must submit a mitigation review for *every High and Medium finding* from the parent audit that is listed as in-scope for the mitigation review. **Incomplete mitigation reviews will not be eligible for awards.**

## Findings being mitigated

Mitigations of all High and Medium issues will be considered in-scope and listed here.

- [H-01: Development Team might receive less SALT because there is no access control on VestingWallet#release()](https://github.com/code-423n4/2024-01-salty-findings/issues/712)
- [H-02: First Liquidity provider can claim all initial pool rewards](https://github.com/code-423n4/2024-01-salty-findings/issues/614)
- [H-03: The use of spot price by CoreSaltyFeed can lead to price manipulation and undesired liquidations](https://github.com/code-423n4/2024-01-salty-findings/issues/609)
- [H-04: First depositor can break staking-rewards accounting](https://github.com/code-423n4/2024-01-salty-findings/issues/341)
- [H-05: User can evade liquidation by depositing the minimum of tokens and gain time to not be liquidated](https://github.com/code-423n4/2024-01-salty-findings/issues/312)
- [H-06: When borrowers repay USDS, it is sent to the wrong address, allowing anyone to burn Protocol Owned Liquidity and build bad debt for USDS](https://github.com/code-423n4/2024-01-salty-findings/issues/137)

- [M-01: THE USER WHO WITHDRAWS LIQUIDITY FROM A PARTICULAR POOL IS ABLE TO CLAIM MORE REWARDS THAN HE DULY DESERVES BY CAREFULLY SELECTING A decreaseShareAmount VALUE SUCH THAT THE virtualRewardsToRemove IS ROUNDED DOWN TO ZERO](https://github.com/code-423n4/2024-01-salty-findings/issues/1021)
- [M-02: Persistent Contract Call revert prevents finalizing a ballot](https://github.com/code-423n4/2024-01-salty-findings/issues/1009)
- [M-03: Creation of token whitelisting proposals can be DOS'd](https://github.com/code-423n4/2024-01-salty-findings/issues/991)
- [M-04: If there is only one USDS borrower, he can never be liquidated](https://github.com/code-423n4/2024-01-salty-findings/issues/912)
- [M-05: Absence of autonomous mechanism for selling collateral assets in the external market in exchange for USDS will cause undercollateralization during market crashes and will cause USDS to depeg.](https://github.com/code-423n4/2024-01-salty-findings/issues/905)
- [M-06: Reusing a SALT that has already been used for voting can allow a malicious proposal to pass and compromise the protocol.](https://github.com/code-423n4/2024-01-salty-findings/issues/844)
- [M-07: Impossible to change managed wallets with proposeWallets after first rejection](https://github.com/code-423n4/2024-01-salty-findings/issues/838)
- [M-08: PriceFeed is likely to be disabled in times of volatility, causing liquidations and borrows to freeze](https://github.com/code-423n4/2024-01-salty-findings/issues/809)
- [M-09: Remove Liquidity has missing reserve1 DUST check, which can make reserve1 to be less than DUST](https://github.com/code-423n4/2024-01-salty-findings/issues/784)
- [M-10: Unwhitelisting does not clear _arbitrageProfits, so re-whitelisting may result in an unfair distribution of liquidity rewards.](https://github.com/code-423n4/2024-01-salty-findings/issues/752)

- [M-11: Title](link to Github issue)
- [M-12: Title](link to Github issue)
- [M-13: Title](link to Github issue)
- [M-14: Title](link to Github issue)
- [M-15: Title](link to Github issue)
- [M-16: Title](link to Github issue)
- [M-17: Title](link to Github issue)
- [M-18: Title](link to Github issue)
- [M-19: Title](link to Github issue)
- [M-20: Title](link to Github issue)

- [M-21: Title](link to Github issue)
- [M-22: Title](link to Github issue)
- [M-23: Title](link to Github issue)
- [M-24: Title](link to Github issue)
- [M-25: Title](link to Github issue)
- [M-26: Title](link to Github issue)
- [M-27: Title](link to Github issue)
- [M-28: Title](link to Github issue)
- [M-29: Title](link to Github issue)
- [M-30: Title](link to Github issue)

- [M-31: Title](link to Github issue)
- [M-32: Title](link to Github issue)
- [M-33: Title](link to Github issue)
- [M-34: Title](link to Github issue)
- [M-35: Title](link to Github issue)
- [M-36: Title](link to Github issue)

[ ⭐️ SPONSORS ADD INFO HERE ]

## Overview of changes

Please provide context about the mitigations that were applied if applicable and identify any areas of specific concern.

## Mitigations to be reviewed

### Branch
[ ⭐️ SPONSORS ADD A LINK TO THE BRANCH IN YOUR REPO CONTAINING ALL PRS ]

### Individual PRs
[ ⭐️ SPONSORS ADD ALL RELEVANT PRs TO THE TABLE BELOW:]

Wherever possible, mitigations should be provided in separate pull requests, one per issue. If that is not possible (e.g. because several audit findings stem from the same core problem), then please link the PR to all relevant issues in your findings repo. 

| URL | Mitigation of | Purpose | 
| ----------- | ------------- | ----------- |
| https://github.com/your-repo/sample-contracts/pull/XXX | H-01 | This mitigation does XYZ | 

## Out of Scope

Please list any High and Medium issues that were judged as valid but you have chosen not to fix.
