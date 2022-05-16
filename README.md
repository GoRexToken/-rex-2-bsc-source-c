# rex-2-bsc-source-c (feedback2)

We have changed the tokenomics:
UPDATED PAPER: https://internet-bonds.com/paper2

REX_REX.sol:
- 25% more Shares (TREX)
- 25% more Shares (irrevocable Stakes)
- no SharePriceUpdate() when withdrawRewards (not necessary)
- precision fixed in stakesShares() and added "initialShares" for each stake (to calculate correct new sharePrice)

REX_RDA.sol:
- changed the daily "addLiquidity" to "every transaction" (capped) to avoid sandwich attacks)


****

Devs contact person: Thomas Rexroth
+ TG: https://t.me/Thomas_REX_ROTH
+ E-mail: go@rex-token.com
