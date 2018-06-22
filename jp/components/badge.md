﻿---
title: Badge - デザイン システム コンポーネント
_description: Badge コンポーネント シンボルは、追加情報のヒントを提供するコンプリメンタリ要素です。
_keywords: デザイン システム, Sketch, Ignite UI for Angular, コンポーネント, UI ライブラリ, ウィジェット
_language: ja
---

## Badge

Badge コンポーネント シンボルを使用して他のインターフェイス要素や通知を表示するために注意を促します。コンポーネントに対するインタラクションに応じてユーザーに追加情報を公開することにより  UX を向上できます。Badge は、[Ignite UI for Angular Badge コンポーネント](https://jp.infragistics.com/products/ignite-ui-angular/angular/components/badge.html)と視覚的に同じものです。

### Badge デモ

![](../images/badge_demo.png)

### 図形

Badge には、円形と四角形の 2 つの異なる図形があります。

![](../images/badge_shapes.png)

### タイプ

Badge は、**数字**やアイコンなど、さまざまなタイプのコンテンツを使用できます。

![](../images/badge_type.png)

### スタイル設定

Badge は、さまざまなオーバーライドで背景、境界線の色、元になるインターフェイス要素でキャストされた影の表示の制御などスタイル設定に柔軟性があります。

![](../images/badge_styling.png)

## 使用方法

Badge を使用して Avatar やテキスト タイトルなどのその他の UI 部分に印を付けます。Badge をそれ自体には使用しないでください。

| いい例                           | 悪い例                         |
| ---------------------------- | ------------------------------ |
| ![](../images/badge_do1.png) | ![](../images/badge_dont1.png) |

## コードの生成

Badge に色を指定した場合、Badge HTML 要素は div でラップされます。ブラウザーによってネスト コンポーネント (他のコンポーネント内のコンポーネント) のスタイル設定が要求されます。

> [!WARNING]
> デザインの Badge のインスタンスで`シンボルからデタッチ`をトリガーすると、ほとんどの場合で Badge のためのコード生成機能が失われる結果となります。

### データ バインディング

データ バインディングは波括弧構文によって指定されます。例: {isAdmin}。テキスト フィールド (`🕹️DataProperty` および `🕹️DataSource` 以外) も文字列補間構文をサポートします。例: 管理者: {isAdmin}。データ バインディングはネストまたはネストなしが可能です。ターゲット プロパティがネストされたプロパティの場合、ネストされたプロパティ チェーンを含みますがモデル オブジェクト名は含みません。実例:

#### ネストなし

```typescript
Customer {
  imageName: String;
}
```
DataProperty: `{imageName}`

#### ネストあり

```typescript
Profile {
  imageName: String;
}

Customer {
  profile: Profile;
}
```
DataProperty: `{profile.imageName}`

### Event プロパティ

`🕹️Event` プロパティはコンポーネント TypeScript のメソッドを作成するために使用されて HTML に Angular クリック シグネチャーを追加します。波括弧構文 ({onEventName}) を使用してイベントを指定する必要があります。

### データ プロパティ

`🕹️DataProperty` 値はバッジ値プロパティへのデータ バインディングを設定するために使用されます。`🕹️DataProperty` はオプションです。`🕹️DataProperty` は、生成要求で提供されるモデル オブジェクト名で指定されたデータ オブジェクトのプロパティ名です。バッジ タイプを Icon に設定した場合、`🕹️DataProperty` は無視されます。

### タイプ

バッジが数値/テキストまたはアイコンかどうかを決定します。

### テキスト

Type を Number に設定する場合、以下が適用されます。

- `🕹️DataProperty` が提供された場合、値は指定したプロパティにデータ バインドされます。
- Text にデータ バインディングがある場合、値は指定したプロパティにデータ バインドされます。
- Text に値がある場合、値はテキストに設定されます。

## その他のリソース

関連トピック:

- [Avatar + Badge](avatar+badge.md)
  <div class="divider--half"></div>

コミュニティに参加して新しいアイデアをご提案ください。

- [Indigo Design **GitHub** (英語)](https://github.com/IgniteUI/design-system-docfx)