# Ubuntu in Termux

These are scripts that allow you to install Ubuntu 24.04 or 22.04 into your Termux application without the need for a rooted device, Run things like https://ollama.ai inside of Ubuntu locally on your Android device!

## OS Available
- Ubuntu 24.04 (Noble) (24.sh)
- Ubuntu 22.04 (Jammy) (22.sh)

### Installation steps

1. Update and Upgrade Termux: `apt update && apt upgrade -y`
2. Install wget, proot, and git: `apt install wget proot git -y`
3. Go to your HOME folder: `cd ~`
4. Download script: `git clone https://github.com/metaspartan/ubuntu`
5. Go to script folder: `cd ubuntu`
6. Give execution permission: `chmod +x 24.sh`
7. Run the script: `./24.sh -y`
8. Launch Ubuntu: `./startubuntu.sh`

## Install Ollama

1. Update Ubuntu: `apt update && apt upgrade -y`
2. Install deps: `apt install git wget curl jq`
3. Install Ollama: `curl -fsSL https://ollama.com/install.sh | sh`
4. Start Ollama: `ollama serve &`
5. Run a model that will work for your device like Qwen2:0.5b: `ollama run qwen2:0.5b --verbose`

## Important

**• If you have to use ubuntu in termux with a x86/i\*86 architecture or prefer ubuntu 19.10 you can use this branch -> https://github.com/MFDGaming/ubuntu-in-termux/tree/ubuntu19.10**

**• If you get an error message that says "Fatal Kernel too old" you have to uncomment the line that reads "command+=" -k 4.14.81"" (remove the # that is located in front of the line) in the "startubuntu.sh" file**


## Credits

https://github.com/MFDGaming/ubuntu-in-termux for the original source

Carsen Klock https://x.com/carsenklock
