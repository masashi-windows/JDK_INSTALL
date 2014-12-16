***
ＪＤＫのインストールと環境変数の設定(Windowsの場合)
***

Javaのサンプルソースを見るだけならランタイムだけあればいいですが  
自分でJavaやAndroidアプリの開発をするなら、まずJava SEのJDKをインストールします。

 Java SE ・・・Java Standard Edition  
 JDK　　   ・・・Java DevelopmentKit  

下記のリンクからＪＤＫをダウンロードするサイトへ移動。  
[http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

![01](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/01.png)

「こちら(ＵＳサイト)」のリンクでページ移動

![02](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/02.png)

Java Platform (JDK) 8u25のダウンロードボタンをクリック

Java SE Development Kit 8 Downloadsのページに遷移します。

![03](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/03.png)

ページをスクロールすると
真ん中あたりのライセンス同意の
ラジオボタンがあります。

![04](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/04.png)

```○Accept License Agreement```

これを選択するとダウンロードリンクが有効になります。

![05](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/05.png)

お使いのマシンがWindowsの場合  
32bitマシンなら　Windows x86  
64bitマシンなら　Windows x64  
のDownloadリンクをクリックします。


![06](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/06.png)

「ファイルを保存」でダウンロードします。

![07](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/07.png)
ダウンロードしたexeをダブルクリックして
インストールを開始します。

デフォルトの設定でインストールした場合
「C:\Program Files\Java\jdk1.8.0_25\bin」に
JDKがインストールされます。

![08](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/08.png)

この場所へのパスをＰＣの環境変数に設定します。

[コントロールパネル]－[システム]－[システムの詳細設定]から
システムのプロパティウインドウを開き、「環境変数」ボタンをクリック

![09](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/09.png)

「システム環境変数」のPathを選択して「編集」ボタンを押下します。

![10](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/10.png)

「変数値」に設定されている値の一番後ろに
セミコロン「;」を追加して
JDKをインストールした場所を追記します。

 「;C:\Program Files\Java\jdk1.8.0_25\bin」

![11](https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/11.png)

ＯＫで変更を反映させます。


コマンドプロンプトから  
```>java -version```   
と入力して

 java version "1.8.0.25"  
と出ればインストールとパスの設定は完了です。

![12](https://github.com/miyake-yasunaga/JDK_INSTALL/https://github.com/wiki/miyake-yasunaga/JDK_INSTALL/images/12.png)

（wikiにimagesフォルダ作成して画像upしようとしたら
fatal: remote error: access denied or repository not exported
というエラーでフォルダ作れませんでした...画像はまた後ほど。）
