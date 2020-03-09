# [Youtube Uploader Bot](https://t.me/fortizeryou2be_bot)




> Simple [Telegram Bot](https://core.telegram.org/bots "Telegram Bots") to Upload videos to [Youtube](https://youtube.com "Youtube") written in Python3.


### Contents

* [Info](#info)
* [Libraries Used](#libraries-used)
* [Status](#status)
* [Special Notes](#special-notes)
* [Contact](#contact)

### Info

This is a simple hobby project which i was really curious about to impliment. This is a Telegram bot which uses [Youtube Data API v3](https://developers.google.com/youtube/v3/ "Youtube Data API v3") to upload videos to Youtube. This bot uses [OAuth 2.0](https://en.wikipedia.org/wiki/OAuth#OAuth_2.0 "OAuth 2,0") to connect to your Youtube Channel.

### Libraries Used

<details>
           <summary>Pyrogram</summary>
           <p><a href="https://github.com/pyrogram/pyrogram">Pyrogram</a> is used to connect the bot with telegram servers.</p>
</details>
<details>
           <summary>Google Client API</summary>
           <p><a href="https://github.com/googleapis/google-api-python-client">Google Client API</a> is used to connect the bot with Google and then with Youtube.</p>
</details>

### Setup

:heavy_exclamation_mark: This project requires [Python3.7](https://www.python.org/downloads/release/python-370 "Python3.7") (as this was written and tested with Python 3.7.3, try and see if it works with other versions)

**Clone and setup virtual environment**

``` bash
$ git clone https://github.com/fortifying/youtube-upfile.git

$ cd utube

$ virtualenv venv

$ source venv/bin/activate

```

**Install requirements**

With all the above procedures done, its time to install our dependencies.
Run :
```bash
$ pip3 install -r requirements.txt
```

**Run bot**

Lets run our bot for the first time!
```bash
$ python3 bot.py
```
If you did everything correctly, the bot should be running. Go do `/start` to see if the bot is live or not. Follow the instructions provided by bot to setup authorisation and to start uploading.


**Or the easy way of directly deploying to heroku**

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/fortifying/youtube-upfile/tree/master)



### Status

This project is actively maintained and will continue so until I'm tired of it.

### Special notes

* With the Youtube Data API you are awarded with 10,000 points of requests. For one video upload it costs 1605 points, regardless of file size, which calculates to about 6 uploads daily. Once you have exhausted your daily points, you have to wait till daily reset. Resets happens at 0:00 PST, i.e. 12:30 IST. So make your uploads count.

* Uploading copyright contents will leads to immediate blocking of the video, and will not be added to your `MyVideos` section of youtube. But still the video can be played directly through the link provided by the bot.

* All the videos are uploaded as private. You may change it after youtube processes the video.

### Contact

Share the FeedBack and Suggestions with me.
You can contact me [Here](https://telegram.dog/fortifying "Contact me")
