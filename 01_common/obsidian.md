# [[obsidian]]

# settingのリポジトリ
https://github.com/myao9494/obsidian_setting_myao

会社で共用できるように、設定だけは、githhubにあげることにする。以下のボタンでコピーされる
```button
name 設定をコピー
type command
action Shell Commands: Execute: Copy Obsidian Settings
class my-copy-button
```

## これで行こう

https://github.com/amatzk/obsidian-dagnetz-system

階層構造を捨てる。これに時間がかかっているのは否めない

## 個人のリポジトリ

http://100.123.239.15:8080/root/obsidian



## 除外ファイルの設定方法
 - obsidianの設定でできる
	- .obsidian/app.json
		- userIgnoreFiltersでリスト管理されている
	- GUI
		- 設定→ファイルとリンク → 除外ファイル
- omnisaerchにも効くらしい
# ObsidianでNAS上のファイルへリンクする

WindowsのNAS（ネットワークドライブ）上のファイルへObsidianからリンクを貼る場合、標準のパス形式ではうまく機能しないことがある。

## 問題
`\\nas99\仮課\personel` のようなUNCパス形式のリンクが正しく動作しない。

## 解決策
`File path to URI` というコミュニティプラグインを使用する。

このプラグインは、`\\nas99\仮課\personel\test.pdf` のようなWindowsパスを、Obsidianが解釈できる `file:////nas99/仮課/personel/test.pdf` というURI形式に自動で変換してくれる。

これにより、ObsidianのノートからNAS上のファイルへ直接リンクできるようになる。

#技術 #Obsidian #NAS #Windows #ファイルリンク
