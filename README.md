# J.A.R.V.I.S (Just A Rather Very Intelligent System) 
This is a telegram bot made for enhancing user specifications. I created this userbot with help of several other userbots available in telegram.

For any queries or want to get know how it works! 
Thanks to @halto_tha and snapdragon

# WARNING!!!
# FORK AT YOUR OWN RISK

## Installation process

### The Easiest Way

[![Deploy To Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

### The Git command 

Simply clone the repository and run the main file:
```sh
git clone https://github.com/neerajregmi10/jarvis
cd jarvis
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
# <Create local_config.py with variables as given below>
python3 -m userbot
```

An example of file it could be:`local_config.py` 

**Not All of the variables are mandatory**

__The Userbot should work by setting only the first two variables__

```python3
from heroku_config import Var

class Development(Var):
  APP_ID = 6
  API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
```

### UniBorg Configuration

The UniBorg Config is situated in `userbot/uniborgConfig.py`.

**Heroku Configuration**
Simply just leave the Config as it is.

**Local Configuration**
Fortunately there are no Mandatory vars for the UniBorg Support Config.

## Mandatory Vars

-> Only two of the environment variables are mandatory.
-> This is because of `telethon.errors.rpc_error_list.ApiIdPublishedFloodError`
    => `APP_ID`:   You can get this value from https://my.telegram.org
    => `API_HASH`:   You can get this value from https://my.telegram.org
-> The userbot will not work without setting the mandatory vars.
