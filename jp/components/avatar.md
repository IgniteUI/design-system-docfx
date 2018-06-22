﻿---
title: Avatar - デザイン システム コンポーネント
_description: Avatar コンポーネント シンボルは、個人情報を画像で表します。
_keywords: デザイン システム, Sketch, Ignite UI for Angular, コンポーネント, UI ライブラリ, ウィジェット
_language: ja
---

## Avatar

Avatar コンポーネント シンボルは、プロフィール写真、アイコン、イニシャル (文字列) で人をグラフィックで表現するために使用します。Avatar は、 [Ignite UI for Angular Avatar コンポーネント](https://jp.infragistics.com/products/ignite-ui-angular/angular/components/avatar.html)と視覚的に同じものです。

### Avatar デモ

![](../images/avatar_demo.png)

### サイズ

Avatar のサイズは 3 つあります。

- ラージ - プロフィール ページに適しています。
- ミディアム - カスタム メニューや可視化に適しています。
- スモール - コンタクト リストや繰り返しのシナリオに簡単に組み込めます。

![](../images/avatar_sizes.png)

### タイプ

Avatar は、**画像**、イニシャルの文字列、アイコンなど、さまざまなタイプのコンテンツを使用できます。

![](../images/avatar_content.png)

アバターは、**円形**と四角形の異なる 2 つの図形があります。

![](../images/avatar_type.png)

### スタイル設定

Avatar は、さまざまなオーバーライドで背景色、イニシャルやアイコン色を制御することにより柔軟にスタイル設定できます。

![](../images/avatar_styling.png)

## 使用方法

Avatar でイニシャルやアイコンを使用する場合に Avatar 背景色とのコントラストの高い色を選択します。同色の同様の色合いや色収差を生じる組み合わせなど、コントラストの低い色は避けるようにします。

| いい例                        | 悪い例                          |
| ----------------------------- | ------------------------------- |
| ![](../images/avatar_do1.png) | ![](../images/avatar_dont1.png) |

## コードの生成

Avatar の色またはフォントを指定した場合、Avatar HTML 要素は div でラップされます。これはネスト コンポーネント (他のコンポーネント内のコンポーネント) をスタイル設定する際にブラウザーによって要求されます。

> [!WARNING]
> デザインの Avatar のインスタンスで`シンボルからデタッチ`をトリガーすると、ほとんどの場合で Avatar のためのコード生成機能が失われます。

### データ バインディング

データ バインディングは波括弧構文によって指定されます。例: {isAdmin}。データ バインディングはネストまたはネストなしが可能です。ターゲット プロパティがネストされたプロパティの場合、ネストされたプロパティ チェーンを含みますがモデル オブジェクト名は含みません。実例:

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

このプロパティはコンポーネント TypeScript のメソッドを作成するために使用し、HTML に Angular クリック シグネチャーを追加します。イベントが波括弧構文 ({onEventName}) を使用して指定する必要があります。

| Avatar タイプ       | `🕹️DataProperty`                                                                                                                                                                                                                                |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 写真アバター        | このプロパティは、画像ソースにデータ バインドするために使用できます。提供された場合、生成要求で提供されるモデル オブジェクト名で指定されたデータ オブジェクトでプロパティ名になります。                                                         |
| アイコン アバター   | このプロパティは無視されます。                                                                                                                                                                                                                  |
| イニシャル アバター | このプロパティは初期プロパティのバインドに使用します。提供された場合、生成要求で提供されるモデル オブジェクト名で指定されたデータ オブジェクトでプロパティ名になります。Avatar イニシャルは 2 文字のみ描画します。これは Ignite UI の制限です。 |

## その他のリソース

関連トピック:

- [Avatar + Badge](avatar+badge.md)
- [Cards](cards.md)
- [File Upload](fileUpload.md)
- [User Profile](userProfile.md)
  <div class="divider--half"></div>

コミュニティに参加して新しいアイデアをご提案ください。

- [Indigo Design **GitHub** (英語)](https://github.com/IgniteUI/design-system-docfx)