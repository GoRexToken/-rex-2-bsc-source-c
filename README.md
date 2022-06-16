# rex-2-bsc-source-c ( FOR: CertiK and Solidity.Finance)



# LATEST CHANGES 

1.
AUCTIONS / RDA contract:
_fillLiquidityPool() has been added a check for small values when addingLiquidity: "if (_busdAmount >= 1E18)"
to prevent from the contract failing to addLiquidity to PancakeSwap (remainder values like trying to add 0.000000000000000001 BUSD)

2.
Updated the comments sections in the beginning of the contracts

3.
New website online: rex.io


****

The whitepaper has been updated with the details. https://rex.io/paper

****

Devs contact person: Thomas Rexroth
+ TG: https://t.me/Thomas_REX_ROTH
+ E-mail: go@rex-token.com

****

# Project Description / CONTRACTS
REX is a set of 6 smart contracts, made to run on Smart Chain (BSC).

****

1. REX (MAIN contract)

REX token is a STAKING TOKEN - with advanced functions and flexibilty (REX contract) - (uses RDA, DEX, AIRDROP, TREX contracts, used by DEX, AIRDROP, RDA).

FILE: REX_REX.sol (implements REX token, keeps time, provides all staking functions, supports a SharePrice model)

****

2. RDA

REX tokens are (partly) auctioned in 222 DAILY AUCTIONS (DAILY AUCTIONS contract).

FILE: REX_RDA.sol -> implements DAILY AUCTIONS, manages auctions, mints REX, adds liquidity to PancakeSwap (uses REX, MREX)

****

3. DEX

REX STAKES can be sold/bought on a DEX (DEX contract).

FILE: REX_DEX.sol -> implements a decentralized exchange (DEX) for REX STAKES (used by REX, uses REX and MREX)

****

4. AIRDROP

REX CLASSIC holders can claim a REX airdrop (AIRDROP contract).

FILE: REX_AIRDROP.sol -> manages a list of airdrop addresses, mints REX and creates REX STAKES (uses REX)

****

5. TREX

TREX (BEP20) is a supportive token, unlocking special functions in REX.

REX_TREX.sol -> implements TREX, an ERC20/BEP20 token and an own DEX to buy and sell TREX. (Used by REX and DAILY AUCTIONS)

****

6. MREX

MREX (BEP20) is a supportive token, unlocking special functions in REX.

Implements MREX, a simple ERC20/BEP20 token (used by DEX and DAILY AUCTIONS)

(already deployed, in use and "OwnershipRenounced")

https://bscscan.com/address/0x76837d56d1105bb493cddbefeddf136e7c34f0c4

****


# Compiler
We have compiled with

npx oz compile --optimizer on --optimizer-runs 1 --evm-version istanbul


# Website Concept
People use the MAIN WEBSITE (rex.io) to
* Learn about cryptocurrencies, staking, staking strategies, decentralized finance (DeFi) and REX
* Take part in 222 daily AUCTIONS (contract: REX_RDA.sol. They send BUSD and receive liquid or staked REX on the next day.)
* Claim BUSD from Personal Random BigPayDays (after taking part in AUCTIONS).
* Claim referral rewards, REX and BUSD.
* Buy REX via PancakeSwap (or rex.io interface).
* STAKE their REX (REX are burnt, SHARES are created. SHARES earn INTEREST for every staked day.)
* Buy and sell REX STAKES via integrated DEX contract.
* Buy and use TREX (more SHARES in a REX stake, higher limits in auctions,...) and MREX (more REX from auctions and referrals, no fees on DEX,...)
* Claim REX airdrop (liquid or staked REX), if the are in the REX CLASSIC snapshop


# REX TIMELINE :: Project status
https://rextoken.medium.com/rex-project-timeline-a8f01f044831


# All LINKS / Social / Community:
https://linktr.ee/rextoken

