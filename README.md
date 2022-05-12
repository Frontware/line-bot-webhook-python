# LINE bot webhook - LINE Messaging API

webhook for LINE bot, when bot join the group will 

## Getting started local env

```
$ export LINE_CHANNEL_SECRET=YOUR_LINE_CHANNEL_SECRET
$ export LINE_CHANNEL_ACCESS_TOKEN=YOUR_LINE_CHANNEL_ACCESS_TOKEN
$ export ODOO_GROUP_BOT_UPDATE_URL=link to odoo function url

$ pip install -r requirements.txt
```

Run webhook

```
$ python app.py
```

## Getting started with Heroku

### heruku button

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/kpofw/line-bot-sdk-python)

then set Webhook URL: `https://{YOUR_APP}.herokuapp.com/callback`

### deploy by yourself

```sh
heroku create
heroku info # then set Webhook URL: https://{YOUR_APP}.herokuapp.com/callback
heroku config:set LINE_CHANNEL_SECRET="..."
heroku config:set LINE_CHANNEL_ACCESS_TOKEN="..."
git push heroku master
heroku logs
```
