# hardhat-sentio

https://www.npmjs.com/package/@sentio/hardhat-sentio

## Usage

1. Install dependencies

``` bash
yarn add -D @sentio/cli @sentio/hardhat-sentio
```

2. Login with sentio sdk

``` bash
npx sentio login
```

3. Import sentio plugin and specify the project in `hardhat.config.ts`

``` typescript
import "@sentio/hardhat-sentio"

const config: HardhatUserConfig = {
  sentio: {
    project: "longw/default"
  }
}
```

4. Upload and verify contracts with CLI

```
npx hardhat sentio:upload Contract1,Contract2

npx hardhat sentio:verify --contract Contract2 --address 0xF03441E04F1f602e8Eb3ab80735a79880CA05AE6 --chain 137
```
