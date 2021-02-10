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

### SSH接続の確認

```
% ssh -T git@github.com
Hi User! You've successfully authenticated, but GitHub does not provide shell access.
Connection to github.com closed.

% ssh github
Hi User! You've successfully authenticated, but GitHub does not provide shell access.
```

### SSHフォルダのconfig作成

```
% pwd
Users/ユーザー名/.ssh

% vim ~/.ssh/config
```

-> 以下貼付、保存

```
Host github
HostName github.com
User git
IdentityFile ~/.ssh/id_rsa
```

GithubからのSSH鍵でクローン作成

```
git clone git@github.com:Githubユーザー名/リポジトリ名.git
```

# Gitコマンド

#####Github(リモート)から情報を取得・反映

```
% git clone [keyやURL]
# 新規にローカル側にコピーを作成する
```

```
% git pull origin
# ローカル（既存の古い情報）をリモート（最新の情報）と同期する
```
# Gitコマンド

#####Github(リモート)から情報を取得・反映

```
% git clone [keyやURL]
# 新規にローカル側にコピーを作成する
```

```
% git pull origin
# ローカル（既存の古い情報）をリモート（最新の情報）と同期する
```

