# Cardinals Node - Blockchain Core Indexer Desktop Application

## 📖 Introduction

Cardinals Node is a professional blockchain core indexer desktop application designed specifically for macOS systems. This application efficiently indexes and synchronizes blockchain data, providing users with fast and reliable blockchain data query services.

## 🚀 Quick Start

### System Requirements

- **Operating System**: macOS 10.15 (Catalina) or higher
- **Memory**: 8GB or more recommended
- **Storage Space**: At least 10GB of available space (for blockchain data storage)
- **Network**: Stable internet connection

### Download and Installation

1. **Download Application**
   - Visit [Releases page](https://github.com/dogeuni-org/cardinals-node/releases)
   - Download the latest version `.zip` file

2. **Installation Steps**
   ```bash
   # 1. Double-click the downloaded .zip file to extract
   # 2. Drag Cardinals Node to the Applications folder
   # 3. Find and launch the application in the Applications folder
   ```

3. **First Launch**
   - If the system prompts "Cannot verify developer", please follow these steps:
     - Open **System Preferences** > **Security & Privacy**
     - Click **Open Anyway** button
     - Or run in terminal: `sudo xattr -rd com.apple.quarantine /Applications/Cardinals-Core-x86.app`

## 🎯 Usage Tutorial

### Prerequisites: Dogecoin Node Setup

Before using Cardinals Node, you need to install and configure a Dogecoin node first.

#### Step 1: Download and Install Dogecoin Core

1. **Download Dogecoin Core**
   - Visit [Dogecoin Core Releases](https://github.com/dogecoin/dogecoin/releases)
   - Download the latest version for macOS (`.dmg` file)
   - Install Dogecoin Core following the standard macOS installation process

2. **Configure Dogecoin Node**
   
   Create a configuration file `dogecoin.conf` in the Dogecoin data directory:
   
   **Location**: `~/Library/Application Support/Dogecoin/dogecoin.conf`
   
   **Configuration Content**:
   ```conf
   server=1
   txindex=1
   rpcuser=admin
   rpcpassword=admin
   rpcallowip=0.0.0.0/0
   rpcport=22555
   rpcbind=127.0.0.1
   zmqpubhashblock=tcp://0.0.0.0:1222
   ```

3. **Start Dogecoin Node**
   - Launch Dogecoin Core application
   - Wait for the blockchain to sync (this may take several hours for the first time)
   - Ensure the node is fully synchronized before proceeding



