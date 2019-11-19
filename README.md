# LiquidCrypto

## Development

Bootstrapped with [zeus-sdk](https://docs.liquidapps.io/en/stable/developers/zeus-getting-started.html).

### Setup

```
npm install -g @liquidapps/zeus-cmd
```

Only way to do it consistently right now is by bootstrapping with a different service and then manually merging this repo:

```bash
# clone this repo somewhere
git clone liquid-crypto liquid-crypto_

# create a new liquid-crypto dir
mkdir liquid-crypto
cd liquid-crypto
zeus unbox vcpu-dapp-service --no-create-dir

# manually merge this repo to the liquid-crypto dir
# Add cryptoconsumer project to contracts/eos/CMakeLists.txt
# And add a CMakeLists.txt to contracts/eos/cryptoconsumer
```

### Testing

```bash
zeus compile
npm run test-crypto
```
