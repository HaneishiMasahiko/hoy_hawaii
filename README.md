# システム構築演習　Webアプリケーション開発チーム

## チーム名：　ほいハワイ

## アプリ名: School Affair Cloud System (SACS)

## メンバー
* 星野シンジ
* 羽石雅彦
* 渡部晨
* 伊藤謙吾
* 池田達樹

## 目的・解決を目指す問題

* 成績管理の利便性の向上。（定期試験、模試等）
  統計が取りやすくなる。
  紙での管理による煩雑さを削減。
  成績推移等のデータが可視化され、分析しやすくなる。
  教員の実績もわかりやすい。
  
* 印刷代の削減。
* スタッフ（先生）の生産性向上。
* 図書館等のアカウントと統合し、管理を統一する。

## アプリケーションの仕様
### 最低限の機能
#### 生徒
* 定期試験の結果、評価を閲覧ができる。
* 模試の成績の閲覧ができる。
* 閲覧するデータは可視化され、ソートしたり、推移を見たりすることができる。
* 自分の出席状況を確認できる。
* クラス、部活、係等の情報を確認できる。
* 授業で出た課題の一覧を閲覧し、提出状況を確認できる。

#### 教員
* 生徒の基本情報を閲覧できる。
* 生徒の成績、評価等を可視化でき、ソートなどもできる。
* 生徒に対して、課題を出すことができる。
* 生徒の成績入力ができる。

#### 管理者

* 生徒・教員のアカウントを作成できる。

### 発展的な機能
* 図書館のアカウントとの連携（貸し出し状況等が生徒から閲覧できる。）
* 意見箱機能（匿名制）

### 画面遷移・シナリオ

最初に、サイトにアクセスすると、ログイン画面になる。

ログインをすると、生徒用、教師用、管理者用のうち、アカウントに対応したページに遷移する。
ページの大まかな構造としては、左側にメニューが並んでおり、どれかを押すと、右側の内容が変わる。（この際にページロードはせず、javascriptでページを変える。）

### 作業分担

| 作業名         | 主担当者   | 補助担当者A | 補助担当者B |
|----------------|------------|-------------|-------------|
| クライアント側 | 星野シンジ | 渡部晨      |             |
| サーバ側       | 伊藤謙吾   | 羽石雅彦    | 池田達樹    |

### 開発スケジュール

#### クライアント側: 
以下のようなスケジュルで開発を進める。
* 12/21(金): 管理者用、教師用、生徒用の順に、一通りページを作成する。管理者用から先にやるのは、デバッグがしやすくなるからである。
* 01/08(火): 見た目の改善。

これ以降は、適宜サーバ側と話し合いながら、改善をしていく。
* 01/29(火): 完成。

#### サーバ側: 
以下の順序で、開発を進める。
* 12/14(金): ログイン機構を実装する。
* 12/21(金): 学校のテスト、成績のデータ構造を作る。
* 01/08(火): クライアント側の問い合わせに対応を実装。

これ以降は、クライアント側チームと話し合いながら拡張機能の開発。
* 01/29(金) 図書館貸出システム等の拡張機能。

#### 発表準備：
* 01/29(火)-02/01(金): 発表準備。

### 情報

* クラス図: https://www.lucidchart.com/invitations/accept/c7acc212-313e-4e66-9dc6-3c4a08134507
