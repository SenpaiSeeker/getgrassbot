# 🌾 GETGRASS BOT 3X AND 1X - FREE VERSION

**Ultra-Fast Auto Farming Bot with Concurrent Connections**

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Free-green.svg)]()

## 🚀 Features

- ✅ **High Performance** - Up to 1000 concurrent connections
- ✅ **Smart Proxy Management** - Auto removes dead proxies
- ✅ **Live Ping Monitoring** - Real-time connection and ping logs
- ✅ **Multiple Account Support** - Add extra accounts easily
- ✅ **Auto Device Generation** - Creates device IDs automatically
- ✅ **Continuous Operation** - Runs continuously without interruption

## 📋 System Requirements

**Minimum PC Requirements:**
- **RAM:** 512 MB minimum
- **Storage:** 512 MB available space
- **CPU:** 1 core processor
- **Internet:** Stable broadband connection
- **OS:** Windows 10/11, Linux, or macOS

**Python Requirements:**
```bash
pip install aiohttp aiofiles colorama loguru websockets-proxy
```

## 🛠️ Installation

1. **Clone or Download** the bot files
  ```
git clone https://github.com/tonixe/getgrass
cd getgrass
   ``` 
3. **Install dependencies:**
   ```bash
   pip install aiohttp aiofiles colorama loguru websockets-proxy
   ```
4. **Get your User ID** - Check [USERID.md](USERID.md) for detailed instructions
5. **Add your proxies** to `proxy.txt`
6. **Run the bot:**
   ```bash
   python main.py
   ```


## 🔧 Configuration

### Getting Your User ID

**Need help finding your User ID?**
📖 **[Read USERID.md Guide](USERID.md)** - Complete step-by-step instructions

### Adding Multiple Accounts

Edit `config.json` to add extra user accounts:

```json
{
    "user_ids": [
        "your_first_userid",
        "your_second_user_id_here",
        "your_third_user_id_here"
    ],
    "version": "1.0.0",
    "author": "GETGRASS BOT - FREE VERSION"
}
```

**Note:** The first user ID is hardcoded and protected. All additional accounts will work normally with full ping/pong activity and connection management.

## 🌐 Proxy Configuration

### ⚠️ Important Proxy Notice

**DO NOT USE FREE PROXIES** - They are unreliable and may compromise your accounts.

### Recommended Proxy Provider

[![Get Premium Proxies](https://img.shields.io/badge/Get%20Premium%20Proxies-Click%20Here-green.svg?style=for-the-badge)](https://app.proxies.fo/ref/d331ec43-fd97-48cd-7642-3af6b467710a)

**Why choose premium proxies?**
- ✅ High success rates
- ✅ Fast connection speeds
- ✅ 24/7 support
- ✅ Reliable uptime
- ✅ Multiple locations

### Supported Proxy Formats

The bot supports multiple proxy formats. Add them to `proxy.txt` file:

#### 1. **HTTP Proxies**
```
192.168.1.1:8080
203.176.135.102:3128
45.77.177.11:8080
```

#### 2. **HTTP with Authentication**
```
username:password@192.168.1.1:8080
user123:pass456@203.176.135.102:3128
```

#### 3. **HTTPS Proxies**
```
https://192.168.1.1:8080
https://203.176.135.102:3128
```

#### 4. **SOCKS4 Proxies**
```
socks4://192.168.1.1:1080
socks4://203.176.135.102:1080
```

#### 5. **SOCKS5 Proxies**
```
socks5://192.168.1.1:1080
socks5://203.176.135.102:1080
```

#### 6. **SOCKS5 with Authentication**
```
socks5://username:password@192.168.1.1:1080
socks5://user123:pass456@203.176.135.102:1080
```

### Proxy File Example (`proxy.txt`)

```
127.0.0.1:8080
192.168.1.1:3128
10.0.0.1:8888
203.176.135.102:8080
45.77.177.11:3128
185.162.230.55:80
user:pass@91.107.6.115:53281
https://103.148.72.192:80
socks5://134.195.101.26:1081
socks5://user:pass@185.162.229.254:1080
```

## ⚙️ Command Line Options

```bash
# Basic usage
python bot.py

# Custom proxy file
python bot.py -p custom_proxies.txt

# Custom concurrent connections (default: 500)
python bot.py -c 1000

# Custom max connections per user (default: 100)
python bot.py -m 500

# Combined options
python bot.py -p proxies.txt -c 800 -m 200
```

## 🎮 Controls

Once the bot is running:

- **Ctrl+C** - Graceful shutdown
- **View Live Logs** - See real-time ping activity and connections

## 📊 Performance Settings

### Default Settings
- **Concurrent Connections:** 600 simultaneous
- **Max Per User:** 1000 connections
- **Ping Interval:** 25 seconds (faster response)
- **Connection Timeout:** 10 seconds
- **Monitoring Interval:** 3 seconds (high speed)
- **Chunk Size:** 500 connections (ultra-fast batches)

### Optimization Tips

1. **More Quality Proxies = Better Performance**
   - Use 100+ premium proxies for best results
   - Mix different proxy types
   - Use high-quality residential proxies

2. **System Resources**
   - 512MB+ RAM recommended for stable operation
   - Fast internet connection
   - SSD storage for better I/O

3. **Proxy Quality**
   - Test proxies before adding
   - Remove dead proxies regularly
   - Use rotating proxy services

## 🔍 Troubleshooting

### Common Issues

#### Bot Not Starting
```bash
# Check Python version
python --version

# Install missing dependencies
pip install -r requirements.txt

# Check proxy file exists
ls -la proxy.txt
```

#### No Connections
- Verify proxies are working
- Check `proxy.txt` format
- Ensure user IDs are correct
- Check internet connection

#### Low Performance
- Add more quality proxies
- Reduce concurrent connections
- Check system resources
- Use better quality proxies

### Error Messages

| Error | Solution |
|-------|----------|
| `No proxies found` | Add proxies to `proxy.txt` |
| `Connection refused` | Check proxy format and availability |
| `Rate limited` | Reduce connection speed |
| `Authentication failed` | Verify user IDs in config |

## 📈 Monitoring

### Live Monitoring

The bot displays beautiful real-time activity logs with timestamps and colors:
- **Connection Status** - Live connection updates with user identification
- **Ping Activity** - Real-time ping/pong monitoring with device tracking
- **Proxy Management** - Smart proxy removal and optimization
- **Multi-User Support** - Each user account displays separately
- **Performance Metrics** - Active connection counts and batch progress

## 📝 Advanced Usage

### Multiple Instances

Run multiple bot instances:

```bash
# Terminal 1
python bot.py -p proxies1.txt -c 300

# Terminal 2
python bot.py -p proxies2.txt -c 300

# Terminal 3
python bot.py -p proxies3.txt -c 400
```

### Automation Scripts

Create a startup script (`start.sh`):

```bash
#!/bin/bash
cd /path/to/getgrass-bot
python bot.py -c 1000 -m 500
```

## 🤝 Support

### Getting Help

1. **Check this README** - Most questions are answered here
2. **Read USERID.md** - For User ID related issues
3. **Verify setup** - Ensure all files are correct
4. **Test with few proxies** - Start small, scale up
5. **Check logs** - Look for error messages

### Known Limitations

- Maximum 1000 connections per user account
- Proxy quality affects performance
- Some proxy types may not work
- Rate limiting may occur with poor proxies

## 📜 License

This is a **FREE VERSION** of GETGRASS Bot. 

- ✅ Free to use
- ✅ Free to modify
- ✅ Free to distribute
- ❌ Use at your own risk

## 🎯 Tips for Success

1. **Quality over Quantity** - Better to have 50 good proxies than 500 bad ones
2. **Regular Maintenance** - Remove dead proxies weekly
3. **Monitor Performance** - Check connection success rates
4. **Scale Gradually** - Start with fewer connections, increase slowly
5. **Backup Config** - Keep copies of working configurations

## 🚨 Important Risk Notice

⚠️ **USE AT YOUR OWN RISK** ⚠️

- The developer is not responsible for any losses or damages

## 💰 Proxy Services

**Need affordable, high-quality proxies?**

I offer premium proxy services:
- **Price:** $0.70 per 1GB
- **Quality:** High-speed residential proxies
- **Support:** 24/7 customer support
- **Reliability:** 99.9% uptime guarantee

## 📞 Contact & Support

For any questions, issues, or proxy inquiries:

[![Contact on Telegram](https://img.shields.io/badge/Telegram-Contact%20@t6nix-blue.svg?style=for-the-badge&logo=telegram)](https://t.me/t6nix)

**Contact @t6nix for:**
- Technical support
- Proxy purchases ($0.70/GB)
- Setup assistance
- Bug reports

---

**Made with ❤️ for the GETGRASS Community**

*Happy Farming! 🌾*
