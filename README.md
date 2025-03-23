# 📌 How to Install and Use NVM on Linux

This tutorial explains how to **install NVM (Node Version Manager) on Linux**.  
If you already have **Node.js** installed, we will first remove it before proceeding with the installation.  

---

## 📍 1. Check if Node.js is Installed

Run the following command to check if **Node.js** is installed on your system:  

```sh
which node
```
-> If the command returns a path like: `/usr/bin/node`, it means **Node.js is installed**. If not, you can skip the next step and proceed directly to the **NVM** installation.

## 📍 2. Remove Existing Node.js Installation (Optional)

If Node.js is installed and you want to use **NVM** to manage your **Node.js** versions, it's recommended to remove the existing installation.

-> If Node.js was installed using **apt** (Ubuntu/Debian-based systems), run the following commands:

```sh
sudo apt purge nodejs npm -y
```
and 
```sh
sudo apt autoremove -y
```

## 📍 3. Install NVM (Node Version Manager)

Run the following command to install **NVM**.

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash
```

-> This script will **clone the NVM repository** to `~/.nvm` and add the necessary configuration to your shell profile **(~/.bashrc, ~/.zshrc, etc.)**.

- After the installation is done, you can reopen the terminal to use **NVM**.

Check the **NVM** configuration with the following command:

```sh
nvm
```

## 📍 4. Install and apply Node.js version using NVM

Run the following command to install the latest version of **Node.js** `nvm install node`.

OR

--> Use the following command to see **all available Node.js versions in NVM.**
```sh
nvm ls-remote
```

Choose a version and run the command like this:
```sh
nvm install 22.14.0  # Replace with your desired version
```
List Installed **Node.js** versions:
```sh
nvm ls
```
Use a version with the command:
```sh
nvm use 22.14.0 # Replace with your desired version
```