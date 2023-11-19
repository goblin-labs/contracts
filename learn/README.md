## Seed Phrase Generation

`solana-keygen` can be used to generate a new keypair.

```bash
solana-keygen new --no-outfile
```

If the `--no-outfile` flag is omitted, the default behavior is to write the keypair to `~/.config/solana/id.json` resulting in a file system wallet.

```bash
solana-keygen
```
