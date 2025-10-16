<div align="center"><h1>🧱 YBlock</h1></div>

<div align="center">
<h4>Multiplayer game server based on DDNet with account system, economy, and mini-games<h4>

![Version](https://img.shields.io/badge/version-1.0.10-blue?style=for-the-badge&logo=appveyor)
![License](https://img.shields.io/badge/License-Close--Source-red?style=for-the-badge&logo=opensourceinitiative)
![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20-lightgrey?style=for-the-badge&logo=appveyor)
![Language](https://img.shields.io/badge/language-C++-blue?style=for-the-badge&logo=c%2B%2B)
![Issues](https://img.shields.io/badge/issues-0-brightgreen?style=for-the-badge&logo=github)
![Contributors](https://img.shields.io/badge/contributors-5-lightgrey?style=for-the-badge&logo=github)
![Stars](https://img.shields.io/github/stars/IMDelewer/Y-Block?style=for-the-badge&logo=github)
![Last Commit](https://img.shields.io/github/last-commit/IMDelewer/Y-Block?style=for-the-badge&logo=github)
![Wiki](https://img.shields.io/badge/wiki-Documentation-lightgrey?style=for-the-badge&logo=readthedocs)
</div>

---

<div align="center">
  <h2><strong style="color:red;">⚠️ Notice:</strong> This project is closed-source and proprietary.  
  Access is restricted. To request permission, contact <strong>IMDelewer (Ivanov Dmitry) </strong>via 
   Discord (@delewer)</h2>
</div>

---

## 🌐 Supported Languages

- [🇺🇸 English](/docs/readme/English.md)
- [🇷🇺 Русский](/docs/readme/Russian.md)

---

## 🧭 Navigation

- [📋 About the Project](#-about-the-project)
- [✨ Features](#-features)
- [🚀 Installation](#-installation)
- [⚙️ Configuration](#%EF%B8%8F-configuration)
- [📦 Automated Build](#-automated-build)
- [📚 Documentation](#-documentation)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👨‍💻 Author](#‍-author)

---

## 📋 About the Project

YBlock is a modified server based on the DDNet engine with extended features:

- 🔐 Account system with progress saving  
- 💰 In-game economy and banking system  
- 🏗️ Plot system with object management  
- 🎮 Built-in mini-games and duels  
- 🌍 Support for protocols 0.6 and 0.7  
- 🌐 Multilingual support (including Russian)

---

## ✨ Features

### Account System
- Player registration and login  
- Progress saved between sessions  
- File-based data storage (`.acc` format)

### Economy System
- In-game currency  
- Banking operations (deposit/withdraw)  
- Item shop  
- Discounts and temporary items

### Mini-Games
- 1v1 duels with customizable arenas  
- Invitation system  
- Stats tracking

---

## 🚀 Installation

### Requirements
- **Compiler:** GCC 7+, Clang 5+, or MSVC 2017+  
- **CMake:** 3.12 or higher  
- **Python:** 3.x  
- **Libraries:** libcurl, OpenSSL, zlib  

### Quick Start

> THIS IS A CLOSED PROJECT, YOU CANNOT COPY IT

```bash
git clone https://github.com/IMDelewer/YBlock.git --recursive
cd YBlock
sudo apt update
sudo apt install cmake build-essential libcurl4-openssl-dev libfreetype6-dev python3
mkdir build && cd build
cmake ..
make -j$(nproc)
./yblock
```

## ⚙️ Configuration

Create a file `autoexec.cfg` in the root directory:

```cfg
# Main Settings
sv_name "My YBlock Server"
sv_map YBlock
sv_port 8303
sv_max_clients 16

# Account System
sv_login_required 0
sv_acc_folder "data/accounts"

# Economy
sv_bank_modes 1
sv_money_drop_file "data/moneydrops.txt"

# Plots
sv_plot_file "data/plots"
```

## 📦 Automated Build

The project uses GitHub Actions for automatic builds:

- ✅ Automatic compilation for Linux
    
- 📦 Release creation with binaries
    
- 🔄 Manual workflow trigger supported
    

## 📚 Documentation

See [Main Page](/docs/wiki/Main%20Page.md)
    
## 🤝 Contributing

We welcome contributions!

1. Fork the repository
    
2. Create a branch for your feature (`git checkout -b feature/amazing-feature`)
    
3. Commit your changes (`git commit -m 'Add amazing feature'`)
    
4. Push to the branch (`git push origin feature/amazing-feature`)
    
5. Open a Pull Request
    

## 📄 License

MIT License — see **[LICENSE](LICENSE)**

## 👨‍💻 Author

- **[IMDelewer](https://github.com/IMDelewer)**