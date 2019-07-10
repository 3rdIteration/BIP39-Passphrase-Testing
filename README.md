# BIP39-Passphrase-Testing

A collection of tests and dictionary files that can be run to test the secuirty of a BIP39 passphrase using BTCRecover.

For the sake of consistency, the branch of BTCRecover being tested is this one here: https://github.com/madacol/btcrecover/tree/p2wpkh-p2sh (BTCRecover with Segwit Support)

Example 09: 1st Address, Longish Password, all lower case (three tokens)

Passphrase: internationalaccessoriesuniversity

Address we are looking for: 
0x944580c833ca9656978fE59981fdafA08D25572b

Command:

python btcrecover.py --no-dupchecks --tokenlist google-500-english.txt --addr-limit 1 --bip32-path "m/44'/60'/0'/0" --wallet-type ethereum --max-tokens 3

The results that I am after are basically a screenshot similar to this:
https://github.com/3rdIteration/BIP39-Passphrase-Testing/blob/master/Speed%20Comparisons.jpg

You don't need to let it run through to completion, just for about 5 minutes until the ETA stabilises.

