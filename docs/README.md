## Seed Phrase Generation

`solana-keygen` can be used to generate a new keypair.

```bash
solana-keygen new --no-outfile
```

If the `--no-outfile` flag is omitted, the default behavior is to write the keypair to `~/.config/solana/id.json` resulting in a file system wallet.

```bash
solana-keygen new
```

## Public Key Derivation

Public keys can be derived from a seed phrase and a passphrase using `solana-keygen pubkey`.

```bash
solana-keygen pubkey prompt://
```

After entering your seed phrase with `solana-keygen pubkey prompt://` the console will display a string of base-58 characters. This is the _derived_ solana BIP44 wallet address associated with your seed phrase.

Note: You could potentially use different passphrases for the same seed phrase. Each unique passphrase will yield a different keypair.
