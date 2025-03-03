# 包括的グレブナー基底計算プログラム

## 概要

本プロジェクトは、包括的グレブナー基底を計算するプログラムです。\
グレブナー基底は多項式環の理論において重要な概念であり、本プログラムではその包括的バージョンを計算し、初等幾何や包絡線の解析に応用できます。

## 特徴

- 多項式環の包括的グレブナー基底を計算可能
- 計算結果を可視化し、幾何解析をサポート
- 数式処理ソフト Risa/Asir を用いた実装

## 必要な環境

本プログラムは以下の環境で動作します。

Risa/Asir

## インストール

Risa/Asir のインストール方法については、以下の公式サイトを参照してください。

Risa/Asir 公式ページ：
http://www.math.kobe-u.ac.jp/Asir/asir-ja.html

## 使い方

1. User/ox/BGB に PGBMain.rr ファイルを配置します。
2. User/ox/OpenXM/bin/asir を起動します。
3. 以下のコマンドを順に実行します。\
   load("/Users/yokootakuma/ox/BGB/PGBMain.rr");\
   pgbmain(E, N, F, P, V, Ord);
   
   - E, N: パラメータ P の多項式集合
   - F: パラメータ P と変数 V の多項式集合
   - P: パラメータのリスト
   - V: 変数
   - Ord: 項順序（V(E) - V(N) のときの CGS の計算）
5. 結果はリストとして出力されます。

## 入力と出力の例

load("/Users/yokootakuma/ox/BGB/PGBMain.rr");\
pgbmain(E, N, F, P, V, Ord);

## ライセンス

本プロジェクトはMITライセンスのもとで公開されています。

## 貢献

バグ報告や機能改善の提案はGitHubのIssuesで受け付けています。
