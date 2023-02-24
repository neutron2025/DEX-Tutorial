mkdir hardhat-tutorial
cd hardhat-tutorial
npm init --yes
npm install --save-dev hardhat
npm install --save-dev @nomicfoundation/hardhat-toolbox
npx hardhat   选择 Create a Javascript Project
npm install @openzeppelin/contracts

在contracts目录下创建文件 Exchange.sol

npm install dotenv

创建 .env 参数为

QUICKNODE_HTTP_URL="add-quicknode-http-provider-url-here"

PRIVATE_KEY="add-the-private-key-here"

新建 constants文件夹 并在下面创建文件index.js

修改scripts/deploy.js
修改 hardhat.config.js

编译 npx hardhat compile
部署 npx hardhat run scripts/deploy.js --network goerli

---------------------
前端
在目录 DeFi-Exchange下面
npx create-next-app@latest     所有都回车

cd my-app
npm run dev

npm install web3modal
npm i ethers@5

在public 目录下放入图片 cryptodev.svg

修改  styles/Home.modules.css

在my-app下面创建 文件夹constants  在里面创建文件index.js

配置四个值
export const TOKEN_CONTRACT_ABI = "ABI-CRYPTO-DEV-TOKEN-CONTRACT";
export const TOKEN_CONTRACT_ADDRESS = "ADDRESS-OF-CRYPTO-DEV-TOKEN-CONTRACT";
export const EXCHANGE_CONTRACT_ABI = "ABI-EXCHANGE-CONTRACT";
export const EXCHANGE_CONTRACT_ADDRESS = "ADDRESS-EXCHANGE-CONTRACT";

在my-app下面创建 文件夹utils  并在里面创建四个文件 addLiquidity.js, removeLiquidity.js, getAmounts.js, and swap.js

修改文件 pages/index.js