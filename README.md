# Firk
Firk(フィルク)はWindowsアプリ開発をサポートするフレームワークです。

[![Build status](https://ci.appveyor.com/api/projects/status/pwwb2xm9dek1b0ee?svg=true)](https://ci.appveyor.com/project/finalstream/firk)　[![NuGet](https://img.shields.io/nuget/v/Firk.svg?style=plastic)](https://www.nuget.org/packages/Firk/)　[![GitHub license](https://img.shields.io/github/license/finalstream/Firk.svg)]()

FirkはWindowsアプリケーション開発をサポートするフレームワーク＆ライブラリです。  
データベースはSQLiteに対応しています。
データベースを使用しないライトウェイトなコア機能は[Firk.Core](https://github.com/finalstream/Firk.Core)にまとめてあります。

もともと[Movselex](http://www.finalstream.net/movselex/)向けに作成したものですが、
次世代のLinear Audio Playerにも採用する予定です。  
今後、Finalstreamで開発するアプリケーションのフレームワークとして精錬していく予定です。

各アプリごとにAppClientを継承したClientを作成するところからはじまります。  
フレームワークとしての使用方法等は近い将来オープンソースとして公開するMovselexのソースを確認していただければと思います。

##主な機能

###Core
* AppClient(アプリケーションのクライント)
 * 設定ファイル(json)をサポート
 * スレッドセーフ処理実行機構(アクションを処理の単位として特定のスレッドで実行)
 * データベーススキーマアップグレード用アクション
* BackgroundWorker(バックグラウンド処理を実装を支援)

###Database
* DatabaseAccessor(データベースへのアクセスをサポート)
* SQLExecuter(Dapperのラッパ。SQLログ出力)
* SQLiteFunctions
 * GetDirectoryPathSQLiteFunction(ディレクトリパス取得)
 * GetFileSizeSQLiteFunction(ファイルサイズ取得)
 * JoinStringSQLiteFunction(string.joinをSQLで実現)




