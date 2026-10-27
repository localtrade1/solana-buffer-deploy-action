# Solana Buffer Deploy Github Action

<p align="center">
  <a href="https://github.com/Squads-Protocol/solana-buffer-deploy-action/actions"><img alt="action status" src="https://github.com/Squads-Protocol/solana-buffer-deploy-action/workflows/units-test/badge.svg"></a>
</p>

<div align="center">
    <img src="./assets/banner.png" />
</div>

Use this github action to automate Solana program deployments straight from Github. Use in conjunction with https://github.com/Squads-Protocol/squads-program-upgrade.

## Usage

You can consume the action by referencing the `v0.1.6` tag:

```yaml
uses: Squads-Protocol/solana-buffer-deploy-action@v0.1.6
with:
  network: [https://api.devnet.solana.com](https://api.devnet.solana.com)
  program: my_program
  keypair: ${{ env.DEPLOYER_KEYPAIR }}
  program-id: prgCo6HJ2bP8xPJ3zwVnfVbqhBbBgY8t7moykr7wzCx
  buffer-authority: 7CLWzQ3pGwk9TCBnNFVq2p79NGQ8WyhSrrjfXiPN4L9m

## Requirements

The runner must provide `anchor`, `solana`, and `solana-keygen` on `PATH`.

## Development

This is a composite action, so there is no build or packaging step. Edit `action.yml` directly.

See the [actions tab](https://github.com/Squads-Protocol/solana-buffer-deploy-action/actions) for runs of this action! :rocket:
