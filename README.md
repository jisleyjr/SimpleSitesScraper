# XboxBestBuyScraper

# Installation

Use the package manager [pip3](https://www.python.org/download/releases/3.0/) which comes with the installation of python3

### Packages

```bash
pip3 install requests
pip3 install bs4
pip3 install python-dotenv
```

# Usage

If you'd like to use this scraper. You will have to enable 2-step verification through Google.

You will also have to configure your own environment variables as well as a few other variables.

## Environment Variables

Create a `.env` file in the same directory and add these to it
```bash
SLACK_WEB_HOOK = "your own webhook"

^ this can be generated by following the link below
```
[Generate Your Slack WebHook](https://api.slack.com/tutorials/slack-apps-hello-world)
```bash
GOOGLE_APP_PASSWORD = "your own google app password"

^ this can be generate by following the link below
```
[Generate Your Google App Passwords](https://myaccount.google.com/apppasswords?rapt=AEjHL4OXbLfc2ca7f28jSSZ__UkDDMS6my0YHSPwd5_lW1XsFb9HnfpTnud6rEBuWMCbME7_jMPUc34ylkSfrjlpWtpGfd7FAA)

Dont forget to create a `.gitignore` in the same directory and put this inside of it
```bash
.env
```

## Other Variables

```bash
headers = {"User-Agent": 'you can just google search `my user agent` in google and paste it here'}
server.login('your email', GOOGLE_APP_PASSWORD)
server.sendmail('email to send from', 'email to send to', msg)
```
Then just run
```bash
python3 bestbuyscraper.py
```