---
title: "普通の SWI-Prolog 入門"
permalink: /
---

# 普通の SWI-Prolog 入門

[![Deploy Jekyll site to Pages](https://github.com/hsk/normal-prolog-intro/actions/workflows/pages.yml/badge.svg)](https://github.com/hsk/normal-prolog-intro/actions/workflows/pages.yml)
[![View site](https://img.shields.io/badge/view-site-blue)](https://hsk.github.io/normal-prolog-intro/)

## [1. はじめの一歩：Hello World](1.md)

- インストール: SWI-Prologの導入手順
- 最初の述語: hello_world `:- writeln('hello world'). :- halt.`
- コメント

## [2. 変数と条件分岐](2.md)

- 数値: 0,1,2,2.5
- アトム: a,abc, 'hello world'
- リスト: [1,2,3]とか
- 論理変数: 「値を格納する箱」ではなく「未知の空欄（プレースホルダ）」
- 条件分岐: Cond -> Then ; Else によるワンライナーの実装

## [3. ループの書き方](3.md)

- 反復処理: between/3 と forall/2 によるイテレーション
- 集約: findall/3 を使ったリストの生成

## [4. リスト操作の基礎](4.md)

- 構造: [H|T]（HeadとTail）による再帰的データ構造
- 基本操作: member/2 と append/3 の順算・逆算
- 要素抽出: select/3 の活用

## [5. 複合項（構造体）](5.md)

- 複合項とは: 名前（functor）と複数のデータをまとめたもの、アリティ（arity）の説明
- データ分解: 複合項のパターンマッチング
- 分解の別解: =.. によるリストとの相互変換
- DSLとしての活用: 演算子定義による独自の構文生成

## [6. 述語（述語論理としての関数）を作ろう](6.md)

- 設計思想: 戻り値ではなく「引数への書き込み」という考え方
- データベース: 事実（Fact）の記述
- ロジック: ルール（Rule）の定義：:-（ならば）と ,（かつ）
- 特徴: 複数の解を返す述語の仕組み

## [7. パターンマッチによる分岐（switch文）](7.md)

- 節の記述: 複数の節による条件分岐
- 制御: カット演算子 ! によるバックトラックの停止
- 否定: \+（failによる証明）の用法

## [8. 単一化（Unification）：Prologの真髄](8.md)

- 本質: = は代入ではなく「等式の解決」
- 逆算の威力: 方程式を自動解決する論理プログラミングの驚き
- まとめ: なぜ変数は「空欄」だったのか
