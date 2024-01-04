## launching app
* create a tuner_app dir in `/vendor/data/app/scfs/scfs_a/` if it is not available
* copy test.html filefrom the repo to `/vendor/data/app/scfs/scfs_a/tuner_app` and channel.json to `/tmp`
* cd into `tuner_app` and create a symling `ln -s /tmp/channel.json /vendor/data/app/scfs/scfs_a/tuner_app/channel.json`
* disable Selinux -  as a super user run `setenforce 0`
* play watchfree+ on tv
* connect to devtools - <tv ip>:9555 on chrome and select the `smartcast-vnext` link (eg: `devtools://devtools/bundled/inspector.html?ws=10.64.137.207:9555/devtools/page/9E5EA759C78B19229751BBC26F03C0A5` ) and open it in a new tab
* change the address to `127.0.0.1:12345/scfs/tuner_app/test.html` in devtool address bar(left top corner) to launch the app
