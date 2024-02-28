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

- [M-11: SALT staker can get extra voting power by simply unstaking their xSALT](https://github.com/code-423n4/2024-01-salty-findings/issues/716)
- [M-12: DOS of proposals by abusing ballot names without important parameters](https://github.com/code-423n4/2024-01-salty-findings/issues/621)
- [M-13: Adversary can prevent updating price feed addresses by creating poisonous proposals ending in _confirm](https://github.com/code-423n4/2024-01-salty-findings/issues/620)
- [M-14: Ballots not yet past their deadline are incorrectly looped too by tokenWhitelistingBallotWithTheMostVotes()](https://github.com/code-423n4/2024-01-salty-findings/issues/556)
- [M-15: Attacker can take advantage of Chainlink price not occuring within it's 60 minute heartbeat to make PriceAggregator calls fail](https://github.com/code-423n4/2024-01-salty-findings/issues/486)
- [M-16: Suboptimal arbitrage implementation](https://github.com/code-423n4/2024-01-salty-findings/issues/419)
- [M-17: Caller of Upkeep may skip step 11 to save gas](https://github.com/code-423n4/2024-01-salty-findings/issues/383)
- [M-18: _getUniswapTwapWei() will show incorrect price for negative ticks cause it doesn't round up for negative ticks.](https://github.com/code-423n4/2024-01-salty-findings/issues/380)
- [M-19: No proposal time limit traps sponsors of unpopular proposals](https://github.com/code-423n4/2024-01-salty-findings/issues/362)
- [M-20: Some rewards from POL will not be send to team wallet nor burned](https://github.com/code-423n4/2024-01-salty-findings/issues/333)

- [M-21: When forming POL the DAO will end up stucked with DAI and USDS tokens that cannot handle.](https://github.com/code-423n4/2024-01-salty-findings/issues/324)
- [M-22: Minimium Collateral Check Can Be Bypassed](https://github.com/code-423n4/2024-01-salty-findings/issues/279)
- [M-23: StakingRewards pools are not given their promised share of rewards due to incorrect calculation](https://github.com/code-423n4/2024-01-salty-findings/issues/243)
- [M-24: Salt Rewards - Rewards related to Arbitrage profits for pools can be lost](https://github.com/code-423n4/2024-01-salty-findings/issues/239)
- [M-25: Incorrect assumption in PoolMath.sol can cause underflow when zapping is used](https://github.com/code-423n4/2024-01-salty-findings/issues/232)
- [M-26: formPOL lacks slippage and deadline protection](https://github.com/code-423n4/2024-01-salty-findings/issues/224)
- [M-27: Attacker Can Inflate LP Position Value To Create a Bad Debt Loan](https://github.com/code-423n4/2024-01-salty-findings/issues/222)
- [M-28: MinShares Slippage Parameters Are Ineffective For Initial Deposit](https://github.com/code-423n4/2024-01-salty-findings/issues/221)
- [M-29: Incorrect calculation to check remaining ratio after reward in StableConfig.sol](https://github.com/code-423n4/2024-01-salty-findings/issues/118)
- [M-30: Chainlink price feed uses BTC, not WBTC. In case of depegging, oracles will become easier to manipulate.](https://github.com/code-423n4/2024-01-salty-findings/issues/60)
- [M-31: changeWallets() can be confirmed immediately after proposalWallets() by manipulating activeTimelock beforehand](https://github.com/code-423n4/2024-01-salty-findings/issues/49)


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
| https://github.com/othernet-global/salty-io/commit/5766592880737a5e682bb694a3a79e12926d48a5 | H-01 | ManagedWallet has been removed | 

## Out of Scope

Please list any High and Medium issues that were judged as valid but you have chosen not to fix.
