

## Important !

<img width="517" alt="Reason" src="https://i.imgur.com/rD3ujmL.png">
This project is no longer being developed because the project owner lacks high security capabilities, leading to potential security vulnerabilities. Therefore, the project will be permanently suspended.

Special Thanks: 
![image](https://github.com/KanzuXHorizon/Fca-Horizon-Remastered/assets/125113101/0a455054-b7f4-499d-b4b6-c91fd0569ce4)

This package require NodeJS 14.17.0 to work properly.

## Notification !

+ We will have Example Video on Channel "Nguyễn Thái Hảo Official"

Original Project(Deprecated): https://github.com/Schmavery/facebook-chat-api

Wish you a good day!, thank you for using HZI products, best regards

KANZUWAKAZAKI(15/04/2023)

## Support For : 

+ Support English, VietNamese !,
+ All bot if using listenMqtt first.

# Api Cho ChatBot Messenger

Facebook Already Has And Allows Users To Create Api For Chatbots 😪 Here => [Đây Nè](https://developers.facebook.com/docs/messenger-platform).

### This Api Can Make You Payy Acc Like You Never Had Acc, Please Pay Attention =))

Note ! If You Want To Use This Api Please See The Document At [Đây Nè](https://github.com/Schmavery/facebook-chat-api).

## Download 

If You Want To Use It, Download It By:
```bash
npm i fca-imran-remake
```
or
```bash
npm install fca-horizon-remastered
```

Nó Sẽ Tải Vô node_modules (Lib Của Bạn) - Lưu Ý Replit Sẽ Không Hiện Đâu Mà Tìm 😪

### Download Latest Version Or Update
If You Want To Use The Latest Or Updated Version Then Go To Terminal Or Command Promt Enter :
```bash
npm install fca-imran-remake@latest
```
Hoặc
```bash
npm i fca-imran-remake@latest
```

## The benefit of this is that you won't waste time paying and having an account 😪
Please Use With Demo Account => [Facebook Whitehat Accounts](https://www.facebook.com/whitehat/accounts/).

## Using

```javascript
const login = require("fca-imran-remake"); // lấy từ lib ra 

// đăng nhập
login({email: "Gmail Account", password: ""}, (err, api) => {

    if(err) return console.error(err); // trường hợp lỗi

    // tạo bot tự động nhái theo bạn:
    api.listenMqtt((err, message) => {
        api.sendMessage(message.body, message.threadID);
    });

});
```

As a result, it will imitate you as shown below:
<img width="517" alt="screen shot 2016-11-04 at 14 36 00" src="https://cloud.githubusercontent.com/assets/4534692/20023545/f8c24130-a29d-11e6-9ef7-47568bdbc1f2.png">

If You Want Advanced Use Then Use The Bot Types Listed Above!

## List

You Can Read Full Api At => [here] (DOCS.md).

## Settings for Mirai: 

You Need To Go To File Mirai.js, Then Find Line
```js
    var login = require('tùy bot'); 
    /* Có thể là :
        var login = require('@maihuybao/fca-Unofficial');
        var login = require('fca-xuyen-get');
        var login = require('fca-unofficial-force');
    ...   
    */
```

And Replace It With:

```js
    var login = require('fca-imran-remake')
```

After that, run normally  !

## Self-study

If You Want To Research Or Create Your Own Bot, Go To This To Read Its Functions And How To Use => [Link](https://github.com/Schmavery/facebook-chat-api#Unofficial%20Facebook%20Chat%20API)

------------------------------------

### Save Login Information.

To Save, You Need 1 Apstate Type (Cookie, etc,..) To Save Or Use Login Code As Above To Log In!

And this mode is already available in some Vietnamese bots, so you can rest assured !

__Instructions With Appstate__
```js
const fs = require("fs");
const login = require("fca-imran-remake");

var credentials = {email: "FB_EMAIL", password: "FB_PASSWORD"}; // thông tin tk

login(credentials, (err, api) => {
    if(err) return console.error(err);
    // đăng nhập
    fs.writeFileSync('appstate.json', JSON.stringify(api.getAppState(), null,'\t')); //tạo appstate
});
```

Or Easier (Professional) You Can Use => [c3c-fbstate](https://github.com/c3cbot/c3c-fbstate) To Get Fbstate And Rename It Back To Apstate! (appstate.json)

------------------------------------

## FAQS

FAQS => [Link](https://github.com/Schmavery/facebook-chat-api#FAQS)