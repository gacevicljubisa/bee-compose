# README

## Permissions

If needed, set the permissions for the data directories to allow the containers to write to them.

```sh
sudo chown -R 999:999 ./data/bootnode ./data/bee1 ./data/bee2 ./data/bee3 ./data/bee4
```

## Run

```sh
docker compose up -d
```

## Stop

```sh
docker compose down
```

## Fund using Beekeeper

- geth-url is the URL RPC blockchain node
- min-swarm is the minimum amount of Swarm tokens to fund
- min-native is the minimum amount of native tokens to fund
- wallet-key is the private key of the wallet to fund
- addresses is comma-separated list of addresses to fund
- log-verbosity is the verbosity level of the logs (debug, info, warn, error)

```sh
./beekeeper node-funder --geth-url=[rpc_blockchain_endpoint] --min-swarm=10 --min-native=0.1 --log-verbosity=debug --wallet-key=[private_wallet_key] --addresses=0x3a13fca45cbf4afc4f2af2869048fefaf409ba08
```
