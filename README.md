
# 🚀 Blockcast BEACON Node Setup Guide

## 📚 Resources

* 🔗 [Official Guide](https://docs.blockcast.network/main/getting-started/how-do-i-participate-in-the-network/beacon/start-running-your-beacon-today)
* 💬 Join [Adanode Telegram Channel](https://t.me/adanode)

---

## ✅ Prerequisites

Update and install essential tools:

```bash
sudo apt-get update && sudo apt-get upgrade -y
sudo apt install curl git -y
````

Install Docker:

```bash
curl --proto '=https' --tlsv1.2 -sSfL https://raw.githubusercontent.com/Dedenwrg/dependencies/main/docker/docker.sh | sudo sh
```

---

## 📝 Register

1. **[Register here](https://app.blockcast.network?referral-code=IEMPcM)** on Blockcast Dashboard.
2. Go to your profile and:

   * Connect your wallet (Required)
   * Link Twitter & Discord (Optional)
   * Complete quests (Optional)

---

## ⚙️ Run Your Node

Clone the repo and start your node:

```bash
git clone https://github.com/adanothe/blockcast.git
cd blockcast
docker compose up -d
```

---

## 🌍 Get Your Server Location

Get your location:

```bash
curl -s https://ipinfo.io | jq '.city, .region, .country, .loc'
```

---

## 🔐 Register Your nodes

Generate hardware and challenge key:

```bash
docker compose exec blockcastd blockcastd init
```

* Copy the **Registration URL** from your terminal.
* Open it in your browser.
* Your **Hardware ID** and **Challenge Key** will be pre-filled.
* Fill in your location (from the previous command).
* Submit to register your node.

🖼️ Reference image:
![Registration Screenshot](https://docs.blockcast.network/~gitbook/image?url=https%3A%2F%2F3364791352-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FXrwmDBB6htefs8IbVcEc%252Fuploads%252FXJkLd8gHhJGjKbRGh7v5%252FScreenshot%25202025-05-01%2520at%25206.19.08%25E2%2580%25AFPM.png%3Falt%3Dmedia%26token%3Db8a15abb-7cd1-4f9a-9d21-42b8c74b1950\&width=400\&dpr=3\&quality=100\&sign=a575b041\&sv=2)

---

## ⏳ Final Step

Wait a few minutes. Your node will show **Online** on the Dashboard.

---
