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
| https://github.com/othernet-global/salty-io/commit/5766592880737a5e682bb694a3a79e12926d48a5 | H-01 | ManagedWallet has been removed. VestingWallet now just vests directly to teamWallet. | 
| https://github.com/othernet-global/salty-io/commit/4f0c9c6a6e3e4234135ab7119a0e380af3e9776c | H-02 | performUpkeep is now called at the start of BootstrapBallot.finalizeBallot to reset the emissions timers just before liquidity rewards claiming is started.|
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | H-03 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/5f79dc4f0db978202ab7da464b09bf08374ec618 | H-04 | virtualRewards and userShare are now uint256 rather than uint128.|
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | H-05 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | H-06 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/b3b8cb955db2b9f0e47a4964e1e4f833a447a72d | M-01 | virtualRewards now rounded up on _decreaseUserShare |
| https://github.com/othernet-global/salty-io/commit/5f1a5206a04b0f3fe45ad88a311370ce12fb0135 | M-02 | callFromDAO now wrapped in a try/catch |
| https://github.com/othernet-global/salty-io/commit/ccf4368fcf1777894417fccd2771456f3eeaa81c | M-03 | There is now no limit to the number of tokens that can be proposed for whitelisting. Also, any whitelisting proposal that has reached quorum with sufficient approval votes can be executed. |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-04 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-05 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/758349850a994c305a0ab9a151d00e738a5a45a0 | M-06 | ballotMaximumDuration added. There is now a default 30 day period after which ballots can be removed by any user. |
| https://github.com/othernet-global/salty-io/commit/5766592880737a5e682bb694a3a79e12926d48a5 | M-07 | ManagedWallet has been removed. |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-08 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/b01f6e5cb360e89f9e4cdae41d609ea747bcaa86 | M-09 | Fixes reserves DUST check |
| https://github.com/othernet-global/salty-io/commit/c46069644739885fa36e84e27e1dd6362b854663 | M-11 | Ballots now keep track of their own requiredQuorum at the time they were created. |
| https://github.com/othernet-global/salty-io/commit/39921b4a25041c7ac4e9b5279e12bb2ec518140b | M-12 | ballotNames now include all provided proposal arguments. |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-13 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/ccf4368 | M-14 | Removed maxPendingTokensForWhitelisting. There is now no limit to the number of tokens that can be proposed for whitelisting. Also, any whitelisting proposal that has reached quorum with sufficient approval votes can be executed. |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-15 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/a54656dd18135ca57eef7c4bf615b7cdff2613a7 https://github.com/othernet-global/salty-io/commit/53feaeb0d335bd33803f98db022871b48b3f2454 | M-16 | ArbitrageSearch updated as suggested with MSB as well |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-18 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/758349850a994c305a0ab9a151d00e738a5a45a0 | M-19 | There is now a default 30 day period after which ballots can be removed by any user. |
| https://github.com/othernet-global/salty-io/commit/eaf40ef0fa27314c6e674db6830990df68e5d70e | M-20 | POL has been removed from the protocol |
| https://github.com/othernet-global/salty-io/commit/eaf40ef0fa27314c6e674db6830990df68e5d70e | M-21 | POL has been removed from the protocol |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-22 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/44320a8cc9b94de433e437e025f072aa850b995a | M-25 | Zapping no longer uses scaling.  |
| https://github.com/othernet-global/salty-io/commit/eaf40ef0fa27314c6e674db6830990df68e5d70e | M-26 | POL has been removed from the protocol |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-27 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/0bb763cc67e6a30a97d8b157f7e5954692b3dd68 | M-28 | minAddedAmountA and minAddedAmountB are now used. |
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-29 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/8e3231d3f444e9851881d642d6dd03021fade5ed | M-30 | The stablecoin framework has been removed: /stablecoin, /price_feed, WBTC/WETH collateral, PriceAggregator, price feeds and USDS.|
| https://github.com/othernet-global/salty-io/commit/5766592880737a5e682bb694a3a79e12926d48a5 | M-31 | ManagedWallet has been removed. |

## Out of Scope

Please list any High and Medium issues that were judged as valid but you have chosen not to fix. \
M-10 \
M-17 \
M-23 \
M-24

## Additional Scope

### Individual PRs

These are additional changes that will be in scope and were addressed outside of direct mitigation.

| URL | Purpose | 
| ----------- | ----------- |
| https://github.com/othernet-global/salty-io/commit/f16623e6bf1cdb0845b83ebf3592e30885a8fc61 | Arbitrage no longer occurs when zapping liquidity | 
| https://github.com/othernet-global/salty-io/commit/75901cae57382a87b5f049d7afb9c5d9b9ba4c19 https://github.com/othernet-global/salty-io/commit/7de25bca740332ae7a4b2f25c3a6f6419eaa7569 | Arbitrage gas optimization | 
| https://github.com/othernet-global/salty-io/commit/60de2c02bcfbcc64b41c03ea0582ec9e7a3f332a | Gas stabilization by preventing overwriting zeros after performUpkeep | 
| https://github.com/othernet-global/salty-io/commit/6998661013e86a50c7db552d189fadb0521dbeb0 | Fixes arbitrage revert when there is zero SALT/WETH liquidity | 
| https://github.com/othernet-global/salty-io/commit/2d1b7df004394720c0d8bb4aefe903021631eff3 | Limited user swaps to one per block to prevent bypassing arbitrage within a single block | 
