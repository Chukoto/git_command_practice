# git_command_practice

# Gitコマンド練習用リポジトリ

### SSH公開鍵作成

```
% cd ~/.ssh
% ssh-keygen
```

### 読み取り属性付与

```
% pwd
Users/ユーザー名/.ssh

% chmod 600 id_rsa
```

### Github Settings -> SSH and GPG keys -> New SSH key

```
title:
任意の名前

key: 次の中身を貼付、保存
```
```
% pwd
Users/ユーザー名/.ssh

% open id_rsa.pub
-> 中身表示
```

