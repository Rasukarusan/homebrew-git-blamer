# git-blamer

# 概要
指定したユーザーが編集したファイルを全て表示する

![demo.gif](https://user-images.githubusercontent.com/17779386/52857893-e719cc00-316b-11e9-8557-ebf97d7b93ac.gif)

# 使い方

.bashrc or .zshrcに追加
```sh
alias git-blamer='sh ~/git-blamer.sh'
```

git管理下のディレクトリ(git管理下ならどこでも良い)で実行
```sh 
$ git-blamer
```

出力
```
/Users/user/app/README.md
/Users/user/app/docker-compose.yml
/Users/user/app/web/Dockerfile
/Users/user/app/web/app/controllers/BaseController.php

Total 4 file found!
```
 
# オプション
```sh
sh git-blamer.sh -l 追加行数
```
`sh git-blamer.sh 20`の場合20行以上追加したファイルのみ出力されます。

