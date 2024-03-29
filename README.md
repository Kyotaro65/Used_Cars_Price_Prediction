# Used_Cars_Price_Prediction

[kaggle上に公開されたUsed Cars Price Predictionというデータセット](https://www.kaggle.com/avikasliwal/used-cars-price-prediction)を用いて、中古車の価格を推論するモデルです。

ローカルにPython等の環境構築をしていなかった頃の作品で、GoogleDrive内でGoogleColabのみを用いて動かす仕様になっております。ご了承ください。

## Google Colaboratoryで開いてください

ファイルを閲覧するなら、Go to File > Used_Cars_Price_Pred > 任意のブランチを選択 の後、ファイルが表示されるフレーム内の Open in Colab を押せばリンクに飛んで Google Colaboratory で開くことができます。

github上でもコードと実行結果を閲覧できますが、Google Colabratoryのほうが見やすく、実際に自ら実行してみるにはGoogle Colabratory等で行う必要があります。

git clone でレポジトリを複製したい場合は、Google Colaboratory上で作成しているので、Google Drive上にレポジトリを複製すると便利です。

Google Drive上でGoogle Colaboratoryのファイルを作成し、以下のコマンドを打ち込んで実行してください。

```
%cd /content/drive/My Drive/
!git clone https://github.com/Kyotaro65/Used_Cars_Price_Prediction.git
```
以上のコマンドを実行するとGoogle Driveのマイドライブ直下にUsed_Cars_Price_Predictionというフォルダが作成され、その中の構造は以下のようになっています。


- Used_Cars_Price_Prediction（フォルダ）
  - .git（フォルダ）
    - ...
  - Used_Cars_Price_Pred.ipynb（ファイル）
  - train-data.csv（ファイル）
  - README.md（ファイル）
  
  
 Used_Cars_Price_Predictionフォルダをマイドライブ直下でなく任意のフォルダ直下に作成したい場合は、コマンド1行目の My Drive/ 以下に任意のフォルダへのパスを追加してください。
 
 git pullは以下のように行ってください。
 ```
%cd /content/drive/My Drive/Used_Cars_Price_Prediction
!git pull
```

Used_Cars_Price_Predictionフォルダをマイドライブ直下でなく他のフォルダ直下に作成した場合は、コマンド1行目のパスを変更してください。

- Google Colaboratory上でコマンドを実行する際、初めのカレントディレクトリはそのGoogle Colabratoryのファイルの存在場所ではなく常にルートディレクトリであるので、
  今開いているGoogle Colaboratoryのファイルの存在場所を基準とした相対パスは使えません。

- Google Colaboratoryのファイル（.ipynbファイル）の作成は、Google Drive上の任意の場所で右クリック -> その他 -> Google Colabratory。
  Google Colaboratoryが選択できない（インストールされていない）場合は、 右クリック -> その他 -> アプリを追加　-> Google Market Placeが開かれるのでGoogle Colabratoryと検索してインストール。
  
## プログラムについて

  
  上記のUsed_Cars_Price_Predictionフォルダ内のUsed_Cars_Price_Pred.ipynbファイルがPythonで記述されたプログラムです。
  
  Google Colaboratoryで開き全て実行すると、train-data.csvファイルが読み込まれ中古車の値段を推論するモデルが構築されます。
  
  最初のコードセルはドライブをマウントするためのもので、ここだけユーザー側に実行結果の指示に従って操作してもらう必要があります。
  
  データはインド市場のものです。
  
  実用的に用いるにはDjangoなどで機械学習アプリを構築する必要がありますが、その環境をまだ整えられていません。
  
  中古車査定をするAIサービス等の構築を目指しています。
