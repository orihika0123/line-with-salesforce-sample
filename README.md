## How to use

1. press the button below. This will lead you to a wizard to create a heroku app from this repository
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

2. follow the wizard and fill the settings depending on what you want to do.

## Advanced usage
In case you want to change some thing, such as bot's talk scripts, follow the guid below.

1. After you complete the steps above, clone the repository to your local and set the `heroku` alias to the app you created above.
```
git clone https://github.com/hrk623/line-with-salesforce-sample.git app_name
cd app_name
heroku git:remote -a app_name
```

2. Edi the code as you wish.

3. commit the changes and push the project to heroku.
```
git add .
git commit -m 'edited script'
git push heroku master
```


## ローカルで動かす場合

#### パッケージインストール
```
npm install
```

#### envファイルを作成
それぞれの値を設定する。

#### 起動
```
npm start
```

#### ローカルサーバを外部公開する
```
ngrok http 5000
```

#### line developerコンソール画面で必要な設定
line channelのwebhook urlに ngrok が定義したurlを設定する
