# Introduction - Install rust and cargo
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Installing Tools - Install Solana-cli
sh -c "$(curl -sSfL https://release.solana.com/v1.7.12/install)
solana --version
cargo install spl-token-cli

# Creating a wallet
solana-keygen new
solana-keygen pubkey 

# Creating your own tokens
spl-token create-token --url https://api.devnet.solana.com

# Minting new tokens
spl-token create-account <token address> --url https://api.devnet.solana.com
spl-token mint <token address> <number of tokens to be minted>

Phantom Wallet  Gj8QkSgwpmmWgURftDZSnZ5C2g4A2yJgdnmwuDX83tRE
Token Address   HXj5BwV5r7wmLD6Z7QQXMfBM4towBULepv14it1eiY87
Current Supply	100,000.000000000
Mint Authority	FBLbvn2vhViCSm98h5dLahV4uVEH3q88xVb5cPEPVboJ
URL             https://explorer.solana.com/address/HXj5BwV5r7wmLD6Z7QQXMfBM4towBULepv14it1eiY87/largest?cluster=devnet
Decimals        9
