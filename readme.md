## 環境構築
* PyCharm
    * ファイルエンコーディングをUTF-8に変更
* venv仮想環境を作成
    * PyCharmのインタプリタ設定
* Zschaler環境への追加設定
    * venvディレクトリ下にpip.ini配置
    * ```python -m pip install --trusted-host pypi.python.org --trusted-host files.pythonhosted.org --trusted-host pypi.org --upgrade pip``` コマンドを実行
* srcディレクトリ作成
* ライブラリをインストール
    * ```pip install slack_sdk -t ./src``` コマンドの実行例
* 必要なライブラリをインストールした後、プロジェクトのルートディレクトリにライブラリ一覧を出力
    * ```pip freeze > requirements.txt```
* 別の環境下でプロジェクトのリポジトリを展開した際には一覧から一括でライブラリをインストール可能
    * ```pip install -r requirements.txt```
    
## PyCharm
### Django
* 開発サーバ起動設定(Chapter5-11 P132)
  * 対象プロジェクトを開き、右上の「構成の追加」をクリックし「実行/デバック構成」を開く
  * Pythonの設定の追加を選び以下の項目を設定
    * Name -> 任意
    * Script path -> private_diaryディレクトリのmanage.pyを選択
    * Parameters -> runserver
    * Environment Variables -> DB_USER,DB_PASSWORDを追加

* DockerによるPostgreSQLサーバの構築


## 参考サイト
* Django
  * ロギング
    * [[Python] Django ログ出力のまとめ - Qiita](https://qiita.com/okoppe8/items/3e8ab77c5801a7d21991)
  
