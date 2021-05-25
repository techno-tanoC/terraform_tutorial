## Chapter 1 - 準備
### 前提
GCPプロジェクトは作成済み、対象GCPプロジェクトのOwner権限を持っているとします。

### `terraform` コマンドのインストール

MacOSであれば `brew` でインストールできます。

個人的には [ `asdf` ](https://github.com/asdf-vm/asdf) を使ってます。

```
git clone https://github.com/asdf-vm/asdf.git ~/.asdf
```

`~/.zshrc` や `~/.bash_profile` に以下を追記

```
. $HOME/.asdf/asdf.sh
```

```
asdf plugin-add terraform https://github.com/asdf-community/asdf-hashicorp.git
asdf install terraform 0.15.4
```

### `gcloud` コマンドのインストール

[Google Cloud SDK のインストール  |  Cloud SDK のドキュメント](https://cloud.google.com/sdk/docs/install?hl=JA) を参考にインストールしてください。

MacOSであれば `brew` でインストールすることもできます。

[Google Cloud SDK を Homebrew で macOS にインストールする - Qiita](https://qiita.com/niwasawa/items/40845748659892231e04)

### gcloudの設定
以下を実行。それぞれ認証を求められます。

```
gcloud auth login
gcloud auth application-default login
```
