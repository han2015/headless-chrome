### For mac
### offical site: https://www.google.com/chrome/canary/
### how to install
download and install directly: https://dl.google.com/release2/q/canary/googlechrome.dmg

### alias chrome="/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome"
### alias chromium="/Applications/Chromium.app/Contents/MacOS/Chromium"
```
alias canary="/Applications/Google\ Chrome\ Canary.app/Contents/MacOS/Google\ Chrome\ Canary"
```

### parameters:
#### --headless background mode
#### --blink-settings=imagesEnabled=false block image 
#### --dump-dom print dom
```
canary --headless --disable-gpu --blink-settings=imagesEnabled=false --print-to-pdf https://www.baidu.com/
```


### how to install headless google-chrome for linux server
```
$ wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
$ sudo dpkg -i google-chrome*
```
#### eg. i download a named 60.0.3112.90_amd64.deb of google-chrome
```$ sudo dpkg -i 60.0.3112.90_amd64.deb```

#### how to find where is the chome app
``` $ which google-chrome-stable ```
then i got /usr/bin/google-chrome-stable, for convenience you can make a alias
```$ alias chrome=/usr/bin/google-chrome-stable```
then eg. 
```chome --headless --disable-gpu --blink-settings=imagesEnabled=false --print-to-pdf https://google.com
```