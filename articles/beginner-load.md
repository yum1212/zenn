---
title: "非エンジニアがGatsby製ブログを使えるようになるまでの1ヶ月"
emoji: "🔰"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: [Gatsby,Git,GitHub,VSCODE]
published: true
---
非エンジニアで、マーケティングディレクターのyumです。

普段はSEMを中心に仕事をしていますが、仕事柄非エンジニアとしてできる範囲でWEBサイトの編集を行います。

HTML,CSSの知識は持ち合わせており、PHPも一応読めるし書く時がググりながらできるくらいのレベルです。CSSにおいてはTailwindが大好き。

WordPressはもうじき触り始めて10年くらいになるので、ある程度のことは理解しているつもりです。

## プロローグ

私はもともと[GamePicks](https://gamepicks.tokyo)というPS4を中心としてゲーム攻略サイトを個人で運営していました。

月間20万PV程度のゆるくやっていたサイトでしたが、訳あってWordPressのDBデータを飛ばしてしまい、集客をしまくっていたコンテンツたちとはおさらばしました。

そこから、WordPressの事が少しづつ嫌いになったわけですが、現在はページエクスペリエンスというものが非常に重要視されており、私自身も重要視しているものの1つ。

サイトの表示速度というのは、使用しているサーバーやユーザーの端末スペック、回線速度、ブラウザなど色々絡みあいますよね。

とはいえ、現代のレンタルサーバーは基本的にどれもSSDかつngixが主流になり、LiteSpeedが少し増えてきているよねといったようなかなり低価格高スペックな時代ですよね。

モバイル回線も4Gで100Mbpsは出ることもあるし、平均しても20〜40Mbpsは出る。

端末のスペックもiPhoneであれば、iPhone7以降の端末なら基本的にWEBブラウジングで困ることって実際なかったりする。

### PageSpeedInsightは違った
でも、PageSpeedInsightは発展途上国をベースとした低回線を前提としたエミュレーターでスコアを出していたりするわけで、4GだからOKみたいなことをすべて許容しているかというとそういうわけでもない。

日本であっても場所によっては3G回線並みに落ちることもあるそんな状況でも、ストレス無く表示できるサイトというのが理想的だ。

そう、WordPressじゃまず無理。

今はWordPressに最適化し、表示速度の速度を売りとするサーバーも出てきたが、結局そうやってバックグラウンドをどうにかしないとダメなんだなってため息が出た。

### WordPressのコストには頭悩まされる
WordPressは御存知の通り、コストが色々とかかりすぎる。
メンテナンスコストはもちろんのことだが、サーバー代もたかが1,000円でも年間で12,000円、10年で12万円だ。

なんだか納得できなくなってきて、他になにか良いCMSは無いかなーと探していたものの、CMSという意味ではWordPress一強。

こういった経緯から脱WordPressをすべく情報収集していたことが、今につながる。前置きがだいぶ長かったが最近1ヶ月の話を記録として残しておきたいと思う。

## GatsbyJSとの出会い
2年前だかそれくらいに、GatsbyJSに出会った。

この表示速度、ページ遷移スピードに感動しどうにか扱えるようになりたいと思った。

そこで、Netlify,Vercel,GitHubといったものを一緒に知ることとなる。

ひとまず、GatsbyのスターターテンプレートをNetlifyに1クリックでデプロイし、実際にデプロイしたテンプレートを触って感動していたことをいまでも覚えている。

## Gitが扱えないと改修すらできないということを知らなかった
しかし、GatsbyJSはかれこれ4回以上挫折している。

どうにも扱い方が理解できず、リトライしては折れてを繰り返してきた。

[ブログの記事](https://gamepicks.tokyo/gatsbyjs/)にも書いたことだが、Gitを扱えないことが足を引っ張っているというのに気づくまで少なくとも2年かかった。

Gatsbyの解説しているサイトを見ると、よくプラグインをコマンド打ってインストールして〜なんてことを書いているが、わけが分からなかった。

どうにかこうにか、GitHub上で触ろうとしていたあの時の自分に喝を入れてやりたい。

## いまGatsbyに興味を持っている非エンジニアへ
まず、GitとGitHubの使い方をマスターしましょう。話はそれからです。

少なくともこれが扱えれば、ググりながらGatsbyを触れる。

次に、（いま私も勉強中の）Reactが必要になってくる。

よりテクニカルな改修をしたい時は、尚更必要になるだろう。

これに並行してGatsbysそのものを勉強していくことで、より扱えるようになると考えている。

他にもGraphQLとかいうものも理解しておく必要はあるだろうが、これは最後に取っておくことにしている。

ひとまず、いま使っているテンプレートをアップデートするために必要な知識を身につけている段階といったところだ。

これが2年以上挫折していた私の直近1ヶ月の変化だ。

## なぜこんなに急成長したのか？
職場でバージョン管理をすることになり、GitとGitHubが本格的に導入された。

これをきっかけにGitとGitHubの理解が一気に深まり、この2つだけでGatsbyでブログ更新ができるまでになった。

Git,GitHubが使えれば、ひとまずテンプレートを使ってこのようにブログを更新することができる。

少しReactを覚えてくると、自分でAdSenseの追加までできるようになる。

大事なので繰り返し言うが、とにかくGit,GitHubからはじめよう。じゃないといじれない。

脱WordPressをしたい非エンジニアの方に参考になれば幸いです。