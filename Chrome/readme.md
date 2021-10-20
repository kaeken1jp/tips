# extension

[Amazon URL Shortener - Chrome Web Store](https://chrome.google.com/webstore/detail/amazon-url-shortener/bonkcfmjkpdnieejahndognlbogaikdg)

[Instant Data Scraper - Chrome Web Store](https://chrome.google.com/webstore/detail/instant-data-scraper/ofaokhiedipichpaobibbnahnkdoiiah)


# Where to find extensions installed folder for Google Chrome on Mac?

```
~/Library/Application\ Support/Google/Chrome/Default

Go to chrome://extensions/, and find out the ID of an extension (32 lowercase letters) (if not done already, activate "Developer mode" first).

Open the terminal, cd to the directory which is most likely a parent of your Chrome profile (if unsure, try ~ then /).

Run find . -type d -iname "<EXTENSION ID HERE>", for example:

find . -type d -iname jifpbeccnghkjeaalbbjmodiffmgedin
```


# error

## Sheets Stuck at Still Loading when using Chrome Browser

```
Please try (Chrome menu) Settings > Advanced > Reset as that should fix it.
```
