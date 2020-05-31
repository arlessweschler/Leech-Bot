<h1 align="center">Telegram Torrent Leecher 🔥🤖</h1> 
<p align="center">
<a href="#"><img alt="donate" src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png"/></a>
</p>
<p align="center">
<a href="https://img.shields.io/github/issues/imsawankumar/Leech-Bot"><img alt="issues" src="https://img.shields.io/github/issues/imsawankumar/Leech-Bot"/></a>
<a href="https://img.shields.io/github/license/imsawankumar/Leech-Bot"><img alt="license" src="https://img.shields.io/github/license/imsawankumar/Leech-Bot"/></a>
<a href="https://sawankumar.gitlab.io/"><img alt="author" src="https://img.shields.io/badge/author-Sawan%20Kumar-red"/></a>
<a href="https://www.python.org/"><img alt="language" src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg"/></a>
<a href="https://github.com/ellerbrock/open-source-badges/"><img alt="author" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103"/></a>
</p>

<hr>

> ## A Telegram Torrent (and youtube-dl) Leecher based on [Pyrogram](https://github.com/pyrogram/pyrogram)

## Donate 

[<img src="https://raw.githubusercontent.com/imsawankumar/Torrent-Mirror-Bot/master/files/paypal.png">](https://www.paypal.me/sawan1800)
[<img src="https://raw.githubusercontent.com/imsawankumar/Torrent-Mirror-Bot/master/files/upi.png">](#)

## Deploying

### The Easy Way

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

### The Legacy Way
Simply clone the repository and run the main file:

```sh
git clone https://github.com/SpEcHiDe/PublicLeech.git
cd PublicLeech
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
# <Create config.py appropriately>
python3 -m tobrot
```

### An Example of config.py 👇
```py
from tobrot.sample_config import Config

class Config(Config):
  TG_BOT_TOKEN = ""
  APP_ID = 6
  API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
  AUTH_CHANNEL = -1001234567890
```

### Variable Explanations

##### Mandatory Variables

* `TG_BOT_TOKEN`: Create a bot using [@BotFather](https://telegram.dog/BotFather), and get the Telegram API token.

* `APP_ID`
* `API_HASH`: Get these two values from [my.telegram.org/apps](https://my.telegram.org/apps).
* `AUTH_CHANNEL`: Create a Super Group in Telegram, add `@GoogleIMGBot` to the group, and send /id in the chat, to get this value.

##### Optional Configuration Variables

* `DOWNLOAD_LOCATION`

* `MAX_FILE_SIZE`

* `TG_MAX_FILE_SIZE`

* `FREE_USER_MAX_FILE_SIZE`

* `MAX_TG_SPLIT_FILE_SIZE`

* `CHUNK_SIZE`

* `MAX_MESSAGE_LENGTH`

* `PROCESS_MAX_TIMEOUT`

* `ARIA_TWO_STARTED_PORT`

* `EDIT_SLEEP_TIME_OUT`

* `MAX_TIME_TO_WAIT_FOR_TORRENTS_TO_START`

* `FINISHED_PROGRESS_STR`

* `UN_FINISHED_PROGRESS_STR`

* `TG_OFFENSIVE_API`

## Available Commands

* `/ytdl`: This command should be used as reply to a [supported link](https://ytdl-org.github.io/youtube-dl/supportedsites.html)

* `/leech`: This command should be used as reply to a magnetic link, a torrent link, or a direct link. [this command will SPAM the chat and send the downloads a seperate files, if there is more than one file, in the specified torrent]

* `/leech archive`: This command should be used as reply to a magnetic link, a torrent link, or a direct link. [This command will create a .tar.gz file of the output directory, and send the files in the chat, splited into PARTS of 1024MiB each, due to Telegram limitations]


## How to Use?

* Send any one of the available command, as a reply to a valid link.

* Files Larger than 1500MB are splitted into parts, and uploaded to Telegram group. To join the files, Download all the parted files, place them in the same directory.
  
  👉 Windows < 10 Users: 
  
  `Extract the contents of` [Hl-join.zip](https://github.com/imsawankumar/Leech-Bot/hl-join/hl-join.zip)  `into the same directory, and run the the join32.exe to join the files.`
  
  👉 GNU/Linux Users: 
  
  `cat filename.00001 filename.00002 filename.00003 > filename`
   Replace filename in the above command, as required.
  
* If you got a file.tar.gz from the bot:

  👉 Windown 10 Users : 
  
  `Install [7-zip](https://www.7-zip.org/download.html)`
  
  `Extract the .tar.gz file.`
  
  👉 GNU/Linux users : 
  
  `Just right click and select "Extract Here" if you use Ubuntu.`

## Thanks to :heart:

* SpEcHiDe for his [Public Leech](https://github.com/SpEcHiDe/PublicLeech)
* Dan Tès for his [Pyrogram Library](https://github.com/pyrogram/pyrogram)
* Robots for their [UploadBot](https://telegram.dog/UploadBot)
* AjeeshNair for his [torrent.ajee.sh](https://torrent.ajee.sh)
* And gotstc, aryanvikash and HasibulKabir.

