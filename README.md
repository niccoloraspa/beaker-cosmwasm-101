# cosmwasm

## LocalOsmosis

```bash
git clone https://github.com/osmosis-labs/LocalOsmosis 
make startd
```

## Beaker

### Deploy contract

```
beaker wasm deploy counter --signer-account test1 --raw '{ "count": 0 }' --network testnet
```

### Deploy contract from beaker console

```
.deploy counter -- --signer-account test1 --raw '{ "count": 1 }'
```

### Commands in console

```
sc = contract.counter.signer(account.test1)
```

```
sc = contract.counter.signer(account.test1)


await sc.getCount()
await sc.increment()
await sc.decrement()
await sc.decrement()
```

### Restart

```
beaker wasm ts-gen counter
beaker console
```

## Resources

- https://github.com/osmosis-labs/beaker
- https://github.com/CosmWasm/cw-plus