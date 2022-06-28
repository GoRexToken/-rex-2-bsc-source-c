# rex-2-bsc-source-c ( FOR: CertiK and Solidity.Finance)


Dear Auditors, 

All REX contracts have been deployed on Mainnet, initialized and the ownerships have been revoked.
Please find the proof of the "RevokeOwnership" (Txn links) below.

TREX: The contract has been published on bscscan.com.
(We don't mind people copy that code.)

We have NOT "published and verified" the mainnet contracts of "REX", "RDA/AUCTIONS" and "DEX" yet. 
And - frankly - we have decided to do anything possible to keep hiding the code, because we fear it will all be copied right away.
(The website has already been copied and people have been scammed. We managed to get their malicious website offline already / "rextoken.live".)

We want to do anything to protect REX investors and their values.
For that, we asked S.F how it would be possible to show investors, that the DEPLOYED contracts exactly match the AUDITED contracts.
S.F said, it would be possible, that the Auditors deploy the "finalcommit" contracts (REX/RDA/DEX) on testnet themselves - and then compare the BYTECODE to our mainnet deployment.

If that's the case, that this was a perfect proof, we would BEG you to support us doing that - and communicate it that way.  

So: The contracts deployed on Mainnet EXACTLY match the "finalcommit" here.
Can you check and confirm that?

If you could, would it be possible to somehow put that into the reports?

From our point of view, that would be a perfect solution.
The investors understand it's the audited code, but nobody can copy it.

Anyways, we'd love to publish the code in the future - maybe after the "auction phase" in 225 days - because we invented some new things and people should see that.

Please comment on that idea.

THANK YOU SO MUCH!

Please find the mainnet deployment details below.

Best regards
Yonko

[Source of this text: https://github.com/GoRexToken/-rex-2-bsc-source-c/edit/finalcommit/README.md]


# MAINNET DEPLOYMENT DETAILS 

+ REX MAINNET (BSC)

+ LAUNCH 1656608400
+ DAY 0 = Thu Jun 30 2022 17:00:00 GMT+0000 (AUCTIONS start +1 day = 1656694800) // 18:00 LONDON - 12:00 CAYMAN ISLANDS

+ REX 0xb25583E5e2dB32b7FCbffe3f5e8E305C36157E54
+ revokeAccess() https://bscscan.com/tx/0x91a2332906a3dcc3dc54da85fb1403b355e6a2641bb7756b07909141c54bd22f

+ RDA/AUCTIONS 0x0bA69EdF05AbE71028f82202Bb394a64C224dDF5
+ revokeAccess() https://bscscan.com/tx/0x070814ae848a4669ef91fa357d82b90694695530e2a8dd53e92e3afe76dc07f0

+ DEX 0x3D11149b23C90379295681e773864A5a5d2b0D90
+ revokeAccess() https://bscscan.com/tx/0xd9c669d23afcfa0d8e3d92a79a2c1794a0efac4c56c1dabe67437c7cc8ada47e

+ AIRDROP 0xd65b42a7FeF267a2E79cbD3b3C8672C1ECE35828 (around 2,000,000,000 REX airdrop, 6486 addresses)
+ revokeAccess() https://bscscan.com/tx/0xe4559a5dc3f1685fabeacb4be2735cbf4816c2f227c2f7658f486c7faa0cd364

+ TREX 0xA4d97197d7c2FaDf1C8e2226d03AAD8Ac1583b9C (858 airdrop addresses)
+ RenounceOwnership() https://bscscan.com/tx/0xd3eb009b05bce8e4de9edce0721762bd642c9c97db2f723549d162ca0091ece6

+ PAIR REX-BUSD 0x207B298f4e08FaCb491f13E8335969E12c912d3e
+ BUSD 0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56
+ DEPLOYER 0xD7B9F1e2C8E9C3498F4D38A230E4EB227F9C3b3e
+ ROUTER 0x10ED43C718714eb63d5aA57B78B54704E256024E
+ MREX 0x76837D56D1105bb493CDDbEFeDDf136e7c34f0c4


****

Dev: YONKO
+ Dev contact person: Thomas Rexroth
+ TG: https://t.me/Thomas_REX_ROTH
+ E-mail: go@rex-token.com

****

# LATEST test: MAINNET (BSC)
REX contracts
REX 0xbAB3333F619603b92a85AD4d6aB8876A8b2b2DD6

PAIR 0x451E2809e81e992cc94a29Ca399b6F7333995aDE

RDA 0x5047e1Bd460151aa3f2770769b133d3749F775bb

TREX 0x0103f665F65249fE7c914128501248f0b51c29f7

MREX 0x76837D56D1105bb493CDDbEFeDDf136e7c34f0c4

BUSD 0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56

STAKE DEX 0xC4d8c7f449f83adf25A5f24169da516F7488aF45

AIRDROP 0x5979012039E72779cA4992e53DfB38F07018C6a1

COMPENSATION 0x18366969bf6C324Edc0076C9833A1a680909378F

MARKETING-FUND 0x7D0Eea6f05535890Cd515190618222fd72fE735A

DEV-FUND 0xa66d267B19332dA0A6054Ac9F284b8716c864F84

----


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

