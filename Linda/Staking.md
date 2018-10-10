# Linda - Staking
Staking is a process whereby you put your coins in a Linda wallet and hold them. You're paid a return (in Lindacoins) for holding them.

## Requirements
* The coins in your wallet needs to be their for at least 24 hours to mature
* Your wallet has to be fully synced with a decent amount of connections
* Your wallet must be unlocked for staking

## Staking process
* When a wallet stake occurs, the stake payment will be added to the balance of the address that created the stake.
* After a successful stake, the coins require 24 hours to remature.
* If the balance of this address is > 100k Lindacoins then the stake process will split the coins into 2 inputs, each of these inputs will then stake separately on the same wallet address.
* The smaller stake inputs will take more time to gain weight to restake, but will follow the same process as above, again splitting if their value is > 100k.

## Things to note
* Sending coins from a wallet will interupt the staking process of any inputs chosen to fulfill the total amount to send. These interrupted inputs will require 24 hours to remature. It is also likely that any coins of these inputs not sent out will be returned on a new wallet change address.
* If you wish to also use your wallet for regular transactions, create a seperate address for these funds, and use the input selection dialog to choose the coins, this will ensure that staking does not get interrupted.
