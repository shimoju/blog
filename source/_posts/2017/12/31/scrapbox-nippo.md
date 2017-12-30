---
title: Scrapboxでリアルタイム共同日報をやってみた
date: 2017-12-31 08:00:00
categories:
  - 技術
tags:
  - Scrapbox
  - チームビルディング
---

この記事は[GMOペパボ Advent Calendar 2017](https://qiita.com/advent-calendar/2017/pepabo)の17日目……になる予定だった記事です。
担当日に風邪を引いてしまって穴を空けてしまいましたが、なんとか年内に投稿してギリギリセーフの雰囲気を出していこうと思います😇

## 朝会の機能不全

どのようなチームでも、人数が増えてくると「誰が何やってるのかわからない」という状況は起こるのではないかと思います。そのための情報共有の場として朝会はよく実施されていますが、自分のチームでは有効に機能していない状態でした。

- 当初は朝会をやっていたが、チーム6人中フレックス勤務対象者が2人おり、その時間に出勤していないことが多々ある
- 今度は夕会にしたが、会議がその時刻に入って欠席者が出たり、作業に集中していると夕会のことを忘れたりする
- その日にやったことは翌日になると(夕方でも)割と忘れており、シュッと出てこない

また、現在弊社では自由度の高い働き方をしていくための各種施策が進められており、来年には全従業員にフレックス勤務が導入される予定です。在宅勤務の拡大も検討中であり、今後「チーム全員が確実にその場に集まれる状況」はますます減っていくことになります。そのような状況にも対応できるような形にした方がよいと感じていました。

## 共同で、リアルタイムに、無理なく日報を書く

このような課題を感じていたころ、先輩の@yuta25さんが[Scrapboxで共同日報を書く](http://razokulover.hateblo.jp/entry/2017/12/07/200728)という記事を見つけ、よさそうだからやってみないかという話になりました。

[Scrapbox](https://scrapbox.io/)はリアルタイムに共同編集ができるノートアプリで、一言でいえば動作が軽いGoogleドキュメントみたいな感じです。Markdownをより簡単にしたような[Scrapbox記法](https://scrapbox.io/help-jp/%E8%A8%98%E6%B3%95)があります。

共同日報の運用方法はほぼ上記参考記事と同様です。1日ごとにページをひとつ作り、各人が今日やるタスクや作業ログを随時箇条書きで書いていきます。自分のタスクはできるだけ一箇所にまとめるようにします。
アイコンショートカットを行末にいちいち入れるのが面倒なので、アイコンのみの行をひとつ作ってそれ以下はその人のエリア、みたいに示しています。これは明確にルールにしたわけではなく、自然とこうなりました。

面倒くさがりで飽きっぽいひとが(自分も含め)多いチームですが、12月8日から始めて今のところ毎日続いており、これは続きそう！という感触を得られています。

## 良かった点

情報共有の場としては、朝会や日報、[分報](http://c16e.com/1511101558/)などの取り組みがありますが、それらと比較しながら共同日報の良かった点を紹介します。

### 作業負荷が低い

日報ではそれを書くこと自体に結構な時間が費やされてしまいます。文章の形にまとめるのは負荷の高い作業なので、定時間際では疲れで億劫になりますし、「日報残業」になってしまうと本末転倒です。
共同日報では作業ログのような形で随時書いていって、そうしていたらいつの間にか日報ができている、という環境を作れます。箇条書きであれば文章が苦手な人でも書きやすく、続けやすいのではないかと思います。

### 「今日やること・やったこと」なので小さなことも書ける

タスク管理としてTrelloを使っていたこともありますが、粒度の設定がまちまちで、いつまでも動かないタスクが出たりしていました。また、「タスクにならないタスク」が出て、タスク管理してるはずなのにいま何をやってるの？という状態になりがちでした(Trelloが悪いのではなく運用が悪いので、もっとよくできたとは思います…)。
日報という形式のいいところは「今日やったこと」を書くので、チームの業務に関わらない事務作業とか、ランチの内容とか、仕事中の気持ちの面とかも書きやすい点があると思っています。実はそこにボトルネックや改善のヒントがあったりするものです。その利点を活かしつつ、随時書いていくことでToDoリスト的にも使っていくことができます。

### 全員が同じページに書いていくので気付きやすい

チャットを使った「[分報チャンネル](http://c16e.com/1511101558/)」では、全員が全員のチャンネルを見ていないと[喫煙所で重要事項が決定されていた問題](http://stefafafan.hatenablog.com/entry/2017/03/21/130422)が生じることがあります。これを回避しながら分報をうまく機能させるのは難しいのではないかと思います。チーム全員でひとつの分報チャンネルを使う手もありますが、チャットでは時系列に制約されるため、話題が入り乱れたり、ちょっと前の話題には言及しにくかったりします。
共同日報ではひとりにつき1ページではなく全員が同じページに書いていくので、自分が書くときに自然と他人のコメントが目に入ります。時系列ではないので行を入れ替えたり、インデントや改行で適切に話題を整理することもできます。

## 悪かった点

### Markdownじゃない

Markdownじゃないのは最初は面食らいます。アイコンの設定のためにページを作るなど独特の仕様もあるので、既にScrapboxのユーザーがいるほうがスムーズだと思います。
ただし綺麗に文章を整えるような使い方ではないのでそこまで困っていません。箇条書き(行頭でスペースorタブ)とアイコンショートカット(Ctrl+i)さえ覚えれば十分でした。

### 作業ログの粒度を調整するのが難しい

参考記事では「楽しくなって会話がはじまってしまう」「細かく実況しすぎてしまう」とありましたが、今のところそこまでの状況には至っていません。逆にもうちょっと細かくしてもいいかなと感じます。とはいえ細かくしようとして細かくすると途端に面倒になるので、うまい距離のとり方は考えどころです。メンバーの性格にもよるところがあると思います。

## まとめ

- 「チーム全員が確実にその場に集まれる状況」を前提としない、無理なく続けられるような情報共有の場が必要と感じていた
- そのために、Scrapboxを使った共同日報を導入してみた
- 共同でリアルタイムに書くことで、作業負荷が低くメンバーが気付きやすい日報になった

まだ導入して1ヶ月なので結論するには早いですが、今までの形よりも手応えがあり、自分のチームには合っているのではないかと感じています。
チームの状況や好みによって様々な手段がありますが、朝会や日報といった情報共有の取り組みの必要性はどのチームも感じていると思います。その手段のひとつとして共同日報をやってみても面白いかもしれません。