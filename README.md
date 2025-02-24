Unofficial Docker image for [EH Forwarder Bot](https://github.com/ehForwarderBot/ehForwarderBot). Maintained by [Roy Xiang](http://github.com/RoyXiang).。

# Installed Channels and Middlewares

* [efb-telegram-master[tgs]](https://github.com/ehForwarderBot/efb-telegram-master)
* [efb-wechat-slave (forked version)](https://github.com/RoyXiang/efb-wechat-slave/tree/itchat)
* [efb-qq-slave](https://github.com/ehForwarderBot/efb-qq-slave)
* [efb-qq-plugin-go-cqhttp](https://github.com/ehForwarderBot/efb-qq-plugin-go-cqhttp)
* [efb-gpg-middleware](https://github.com/ehForwarderBot/efb-gpg-middleware)
* [efb-msg-blocker-middleware](https://github.com/ehForwarderBot/efb-msg_blocker-middleware)
* [efb-notice-middleware](https://github.com/ehForwarderBot/efb-notice-middleware)
* [efb-patch-middleware](https://github.com/ehForwarderBot/efb-patch-middleware)
* [efb-search-msg-middleware](https://github.com/catbaron0/efb-search_msg-middleware)
* [efb-voice-recog-middleware](https://github.com/ehForwarderBot/efb-voice_recog-middleware)

# Get Started

Start a Docker container by the following command:

```
docker run -d --restart=always \
    --name=ehforwarderbot \
    -e "PUID=1000" \
    -e "PGID=1000" \
    -e "TZ=Asia/Shanghai" \
    -e "EFB_PROFILE=default" \
    -v $(pwd)/.ehforwarderbot:/config \
    ghcr.io/royxiang/ehforwarderbot:latest
```
