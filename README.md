# BIP39-Passphrase-Testing

A collection of tests and dictionary files that can be run to test the secuirty of a BIP39 passphrase using BTCRecover.

Example 09: 1st Address, Longish Password, all lower case (three tokens)
Passphrase: internationalaccessoriesuniversity
Address we are looking for: 
0x944580c833ca9656978fE59981fdafA08D25572b

python btcrecover.py --no-dupchecks --tokenlist google-500-english.txt --addr-limit 1 --bip32-path "m/44'/60'/0'/0" --wallet-type ethereum --max-tokens 3
