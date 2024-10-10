# Real Goats Bot Telegram Automation Script

GoatsBot is an automation script for completing missions, checking in, and spinning the slot machine on the Real Goats Bot Telegram. This script handles multiple accounts, automates login, mission completion, and daily check-ins.

[TELEGRAM CHANNEL](https://t.me/cucumber_scripts)

# Warning
- All risks are borne by the user!
- tgWebAppData (query_id / user_id)  for the goats bot must be updated once every 1 day



## Updates
- **10.10.24** Fixed the error of adding tokens to the token.json

## Register

To use this bot, you need to register it with the Goats Telegram Bot. 

1. Open the bot [t.me/Realgot_real](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61)
2. Click on the "[Start App](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61)" or "[Open App]([url](https://t.me/realgoats_bot/run?startapp=754d1e37-4a72-4a04-8a35-81eb362eba61))" button
3. Install This Real Goats Automations Bot
4. Have Fun 


## Features
- **Watching Ads**: automatically watching ads to earn + 500 GOATS `NEW`
- **Automated Login**: Logs in automatically using account details.
- **Mission Completion**: Completes available missions and collects rewards.
- **Daily Check-in**: Checks in daily and collects rewards.
- **Slot Machine**: Spins the slot machine if coins are available.
- **Multi-account Support**: Automates For multiple accounts listed in `data.txt`.
- **Enable Proxies**: To use proxies, set `use_proxies` to `true` in `config.json`.

## Requirements

- Python 3.7+
- `aiohttp` for asynchronous HTTP requests
- `colorama` for colored output
- Other dependencies listed in `requirements.txt`

## Setup and Installation

### Step 1: Clone the repository
```bash
git clone https://github.com/cucumber-pickle/goatsCum.git
cd goatsCum
```
**Create a virtual environment (optional but recommended)**

 ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
 ```
### Step 2: Install dependencies
You can install the required packages by running the following command:

```bash
pip install -r requirements.txt
```

### Step 3: Configure accounts
Create a `data.txt` file in the root directory.
Add Telegram authentication data for each account on a new line:

1. Use PC/Laptop or Use USB Debugging Phone
2. open the `real goats bot`
3. Inspect Element `(F12)` on the keyboard
4. at the top of the choose "`Application`" 
5. then select "`Session Storage`" 
6. Select the links "`dev.goatsbot.xyz`" and "`tgWebAppData`"
7. Take the value part of "`tgWebAppData`"
8. take the part that looks like this: 

```txt 
query_id=xxxxxxxxx-1
query_id=xxxxxxxxx-2
query_id=xxxxxxxxx-3
```
9. Decode query_id= with https://www.urldecoder.org/
10. add it to `data.txt` file or create it if you dont have one

### Step 4: Modify Configurations (Optional)
The `config.json` file allows you to modify script settings:
account_delay: Time (in seconds) between account operations.
looping: Time (in seconds) before starting a new loop of account runs.

### Configuration
You can adjust the bot's behavior via config.json:

```json
{
    "use_proxies": false,
    "account_delay": 5,
    "looping": 3800
  }  
```
`account_delay`: Delay in seconds between switching accounts.
`looping`: Time in seconds to wait before running all accounts again.

### Format of proxies.txt
The proxies.txt file should contain one proxy per line in the following format:

```ruby
username:password@ip:port
username:password@ip:port
```

### Step 5: Run the script
To start the bot, run:

```bash
python main.py
```

### Additional Information
`The script` uses asyncio for asynchronous operations to handle multiple tasks concurrently.
`Error handling` is implemented to gracefully manage login and mission completion failures.
Proxy Format The proxies should be listed in a `proxies.txt` file with the format `username:password@ip:port`, one proxy per line.
Random Proxy Assignment The script will assign a proxy from the list for each account.


## How to get tgWebAppData (query_id / user_id)

1. Login telegram via portable or web version
2. Launch the bot
3. Press `F12` on the keyboard 
4. Open console
5. Сopy this code in Console for getting tgWebAppData (user= / query=):

```javascript
copy(decodeURIComponent(sessionStorage['telegram-apps/launch-params']).split('tgWebAppData=')[1].split('&tgWebAppStartParam')[0])
```

6. you will get data that looks like this

```
query_id=AA....
user=%7B%22id%....
```
7. add it to `data.txt` file or create it if you dont have one


## This bot helpfull?  Please support me by buying me a coffee: 
``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - BSC (BEP 20)

``` UQBiNbT2cqf5gLwjvfstTYvsScNj-nJZlN2NSmZ97rTcvKz0 ``` - TON

``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - Optimism

``` THaLf1cdEoaA73Kk5yiKmcRwUTuouXjM17 ``` - TRX (TRC 20)

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For questions or support, please contact [CUCUMBER TG CHAT](https://t.me/cucumber_scripts_chat)

