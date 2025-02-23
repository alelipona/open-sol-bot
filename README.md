Here's the translation of your readme file from Chinese to English:

# 🤖 OpenSolBot

A fully open-source trading bot on the Solana chain that supports copy trading and automated trading functions. ⚡️

> 💡 This is an open-source trading bot project, inspired by the GMGN Bot implementation. This project is completely open-source, and you keep the private keys yourself to avoid the risk of asset leakage.

## ⚠️ Disclaimer

This project is intended for personal learning and research use only, and not as a production-level project:

- 🎓 This is a practice work, mainly for learning and research purposes.
- ⚠️ It is not recommended to use it directly in a production environment.
- 📢 The author is not responsible for any losses caused by using this project.
- 💡 If you decide to use this project, please do so at your own risk.

## 🎯 Demonstration

![Trading Bot Demo](https://github.com/user-attachments/assets/a4389538-b317-4858-a41d-b0f374d1a18f)

<details><summary>SWAP</summary>
<p>

![Image](https://github.com/user-attachments/assets/7005e10f-e599-414c-9520-b2e558f9e86b)

</p>
</details>

<details><summary>Copy Trading</summary>
<p>

![Image](https://github.com/user-attachments/assets/653eb952-b8f9-4084-a0d3-42e719cc3043)

</p>
</details>

<details><summary>Monitoring</summary>
<p>

![Image](https://github.com/user-attachments/assets/095f87f9-f95c-437a-b5ff-9a6a19e37fc6)

</p>
</details>

> 💬 Group chat: [https://t.me/chainbuff](https://t.me/chainbuff)
>
> ⚠️ **Warning**: This bot is for test experience only
>
> - ❌ Do not import personal wallet
> - ❌ Do not deposit funds into the wallet
> - 📢 Test data may be cleared at any time
> - 🔬 For functionality demonstration and testing only

## ✨ Main Features

- 💬 Telegram Bot
- 📊 Copy trading function
- 🔍 Monitoring function
- 🎫 Activation code system
- 🔒 Secure and open-source

## 💻 Environment Requirements

- 🐍 Python 3.10+
- 📦 MySQL
- 🗄️ Redis
- 🐳 Docker (Recommended)

## 📥 Quick Start

```bash
git clone https://github.com/mkdir700/open-sol-bot.git
cd open-sol-bot
```

## ⚙️ Configuration Instructions

Copy and edit the configuration file:

```bash
cp example.config.toml config.toml
```

### Necessary Configuration

- `tg_bot.token`: Telegram Bot Token ([How to create Bot Token](https://core.telegram.org/bots#how-do-i-create-a-bot))
- `rpc.endpoints`: List of RPC nodes, it is recommended to use private RPC nodes, such as Helius, Quicknode, etc.
- `api`: API configuration, including [Helius](https://helius.dev) and [Shyft](https://shyft.to), these APIs have a certain amount of free quota, which is enough for personal use.
  ```
  [api]
  helius_api_base_url = "https://api.helius.xyz/v0"
  helius_api_key = ""
  shyft_api_base_url = "https://api.shyft.to"
  shyft_api_key = ""
  ```

> 💡 To achieve faster copy trading speed, the default mode uses `geyser`, and WebSocket subscription mode is also supported.

## 🚀 Usage Instructions

For Podman, use the following commands:

Start:

```bash
make up
```

Stop the service:

```bash
make down
```

<details><summary>For Docker, use the following commands:</summary>
<p>
Start:

```bash
docker compose up -d
```

Stop the service:

```bash
docker compose down
```

</p>
</details>

Update:

```bash
git pull
podman/docker compose up -d --build
```

> When upgrading, it is recommended to use the `--build` parameter to rebuild the container.

Detailed deployment documentation: [https://github.com/mkdir700/open-sol-bot/wiki/Deployment](https://github.com/mkdir700/open-sol-bot/wiki/Deployment)

## ⚠️ Precautions

- 🔒 Ensure the security of private keys in the configuration file
- 💡 It is recommended to test with a small amount of funds first
- 🌟 Ensure the stability and availability of RPC nodes

## 🤝 How to Contribute

We welcome your contributions to this project! If you want to participate in project development, please read our [Contribution Guide](CONTRIBUTING.md) first.

## 🙏 Special Thanks

- The Raydium trading module is based on [AL-THE-BOT-FATHER/raydium_py](https://github.com/AL-THE-BOT-FATHER/raydium_py)
- The Pump trading module is based on [wisarmy/raytx](https://github.com/wisarmy/raytx/blob/main/src/pump.rs)

## 📄 License

[MIT License](./LICENSE)

---

If you have any other questions or need further assistance, feel free to ask! 😊
