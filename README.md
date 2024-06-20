# PHP proxy for Telegram Bot API
![Demo](https://sun9-31.userapi.com/c200424/v200424688/35ab7/AFLyGuRVCAA.jpg)

## Requirements
* PHP >= 5.6 
* SSL

## Demo
新建一个站点，并将你的域名解析到此站点，PHP版本我个人设置的为7.3，Github中提示PHP版本要求≥5.6即可，将Github中的index.php和tgproxy.php放入站点目录中，如图所示，具体步骤不再详细阐述。
![image](https://github.com/Today-to-Lsp/Telegram-bot-api-php-proxy/assets/31529293/a2519ebc-0729-4857-a6f0-a0cc5a7b1721)
![image](https://github.com/Today-to-Lsp/Telegram-bot-api-php-proxy/assets/31529293/486207a6-d513-4e77-862c-f3a91694763c)
![image](https://github.com/Today-to-Lsp/Telegram-bot-api-php-proxy/assets/31529293/6452fa6c-09e9-4010-8594-d4b243b2ca5a)

设置伪静态规则
```
rewrite ^/bot.*$ /tgproxy.php last;
```
![image](https://github.com/Today-to-Lsp/Telegram-bot-api-php-proxy/assets/31529293/631da3fd-b12b-4174-ad66-56d5668108c5)
大功告成，此时访问你刚才所添加的站点的域名，即可
