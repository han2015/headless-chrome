### For MAC OX
=====================
- offical site: https://www.google.com/chrome/canary/

#### how to install
- download and install directly: https://dl.google.com/release2/q/canary/googlechrome.dmg

> alias chrome="/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome"
- alias canary="/Applications/Google\ Chrome\ Canary.app/Contents/MacOS/Google\ Chrome\ Canary"

#### chrome parameters:
- background mode --headless
- block image  --blink-settings=imagesEnabled=false 
- print dom --dump-dom 
```sh
canary --headless --disable-gpu --blink-settings=imagesEnabled=false --print-to-pdf https://www.baidu.com/
```



### For Linux Server
=====================

#### how to install headless google-chrome
```sh
$ wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
$ sudo dpkg -i google-chrome*
```

- eg. i download a named 60.0.3112.90_amd64.deb of google-chrome
```sh
$ sudo dpkg -i 60.0.3112.90_amd64.deb
```

#### how to find where is the chome app
```sh
$ which google-chrome-stable 
```

- then i got /usr/bin/google-chrome-stable, for convenience you can make a alias

```sh 
$ alias chrome=/usr/bin/google-chrome-stable
```

- then
```sh 
chome --headless --disable-gpu --blink-settings=imagesEnabled=false --print-to-pdf https://google.com
```


### refer doc
https://developers.google.com/web/updates/2017/04/headless-chrome
