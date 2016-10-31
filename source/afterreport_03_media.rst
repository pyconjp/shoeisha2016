================================
第3回 メディアチームのPyCon JP 2016
================================

はじめに
===========
執筆担当: @kimura

iOSガイドアプリ
==========
こんにんちは！メディアチームの牟田裕太郎です。

PyCon JP 2016からスタッフ参加で、今年はメインでiOSアプリ開発を担当しました。

.. figure:: /_static/afterreport_03_media/iOSAppStore.png
   :alt: App Store
   :height: 500

   `App Store <https://itunes.apple.com/us/app/pycon-jp-2016/id1149419450>`_  

みなさま使って頂けましたでしょうか？

私のパートでは、モバイルガイドアプリ作成の経緯と実際の開発についてやiOSアプリエンジニアがPyCon JPスタッフをやってみてという点について書こうと思います。
`2日目のLT <https://www.youtube.com/watch?v=cyhFFm3yh14&feature=youtu.be&t=28m19s>`_ や `私個人のブログエントリー <http://yutailang0119.hatenablog.com/entry/2016/09/24/180000>`_ と重複する部分もありますが、ご容赦ください。

モバイルアプリ作成の経緯
----------
モバイルアプリ作成のきっかけは、 `私のなにげないツイート <https://twitter.com/takanory/status/697977277062082560>`_ に座長の鈴木たかのりさんが反応したことでした。
上記ツイートの通り、以前はGuideBookという外部サービスを使っていましたが、せっかくなので初のネイティブアプリ内製をしてみようということになりました。
正直な所、今年はトライアルという気持ちで始まりましたが、想定よりも多くの方に使って頂けたようです。
きちんとリリースして多くの方の元に届いたことを嬉しく思うと共に、別領域の人にもチャレンジできる空気感があることは非常にありがたいことでした。

iOSアプリ作成の進め方
----------
iOSアプリ本体の開発はGitHubの `pyconjp/pyconjp-ios <https://github.com/pyconjp/pyconjp-ios>`_ で行っており、APIは `pyconjp/pyconjp-website <https://github.com/pyconjp/pyconjp-website>`_ に内包されています。
今年は私1人の開発でしたが、基本的にPull Request形式としました。
PyCon JPのJIRAだとスタッフ外から見ることができなくなってしまうため、タスク管理はGItHubのissueを使用しましたが、来年はGitHub projectsを採用しようかと思っています。
ライブラリは `通信 <https://github.com/Alamofire/Foundation>`_ と `MobileDB <https://realm.io/products/swift/>`_ のみ使用し、できる限り自分で作成しました。
どんな機能を提供するべきかの要件定義に時間がかかっていまったため、トークにフォーカスを絞った作りになりましたが、特にブックマーク機能は好評頂けていたようです。
また、デザイナーさんはロゴやTシャツ、パンフレット、Webとタスクを多く抱えていたので、大枠はAndroidのエンジニアと私とで決め、色の調整や画像の作成のみお願いすることとしました。
できるだけiOS Human Interface Guidelineに則った作りをを意識しましたが、デザイン力は今後の課題です...

その他の反省として、

* トーク以外のKeynoteなどがタイムテーブルで見れなかったこと
* WebViewに頼る部分が多かったこと
* Androidアプリと連携が取れなかったこと

などがあります。

他にもアンケートや直接お話した方からも多くのフィードバックや要望を頂き、自分自身もやりたかったことの30%程度しか達成できていないので、継続的に開発を続けていこうと思っています。
(v1.0.0リリース当時はSwift2.2でしたが、現在のdevelopブランチはSwift3.0にバージョンアップ済みです。)

iOSアプリエンジニアの私とPyCon JP
----------
私の本業はiOS/Swiftのエンジニアですが、初めてApple Developer ProgramのOrganization登録を経験できたり、このアプリの開発が始まった当初はまだSwiftに触り始めたばかりだったため、本業にも還元することができたりと、カンファレンスの運営以外にもプラスの経験となりました。

私自身、普段はほとんどPythonを触れる機会がなく、Pythonコミュニティはアウェイでした。
しかし、PyCon JP 2015に参加した際、Pythonコミュニティに関わっている方々の温かみを感じ、2016のスタッフに飛び込んでみました。
Python初心者ながらも、iOSエンジニアとしてPythonコミュニティに貢献できたなら、非常に嬉しいです！
Pythonistaのみなさんも、自分の本領域以外のコミュニティにも、Pythonistaとして力になれることがあると思います。
ぜひ参加してみては如何でしょうか？
来年はもう少しPythonを触りつつも、iOSアプリ開発は続けようと思っていますので、ご期待ください！！！


撮影について
================
メディアチームで撮影を担当していた小松です。
`昨年に引き続き、 <https://codezine.jp/article/detail/9079?p=3>`_ 今年の PyCon JP も臼井さんとの2名体制で行いました。

- `PyCon JP | Flickr <https://www.flickr.com/photos/pyconjp/>`_

今年は臼井さんがフラッシュ、小松がキャプチャーレンズと各々新しいアイテムを持ち込みました。
標準レンズと望遠の2本を切り替えて撮影していたのですが、今年はレンズの切り替えが楽になりました。

.. figure:: /_static/afterreport_03_media/capture_lens.jpg
   :width: 600
   :alt: キャプチャーレンズで腰にレンズを付けている様子
   :target: https://www.flickr.com/photos/pyconjp/29807929786/in/album-72157672957842370/

   腰にレンズを付けている様子

スポンサーブースが撮影的に若干暗かったのですが、臼井さんのフラッシュはかなり威力を発揮していました。

.. figure:: /_static/afterreport_03_media/taken_with_flash.jpg
   :width: 600
   :alt: スポンサーブースフラッシュを焚いて撮影
   :target: https://www.flickr.com/photos/pyconjp/29781106211/in/album-72157672957842370/

   スポンサーブースをフラッシュを焚いて撮影

毎年、PyCon JP では参加者の集合写真を撮っているのですが、今年の集合場所は奥行きのある場所になったため異例の縦撮り写真になりました。この写真が SNS などで共有されていたのを見たとき、縦写真はスマホ向きで良いなと思いましたが、その後各所で使用されているのを見て、Web のパーツとしては横の方が使いやすいなと思いました。

皆さんに手を挙げてもらったのは非常に良い写真になったなと思います。

.. figure:: /_static/afterreport_03_media/group_photo.jpg
   :width: 427
   :alt: 手を挙げて集合写真
   :target: https://www.flickr.com/photos/pyconjp/29848436235/in/album-72157673020428422/

   手を挙げて集合写真

今年は少しずつでも Flickr にあげていこうと思い、会場で写真を撮っては選定を行ってアップロードを行っていましたが、撮る量に対して間に合わず昨年同様スプリントで写真選定thonを行いました。 PyCon JP 2017 ではこの辺りを計画的に行えるようにしたいと思ってます。

それから、PyCon JP で撮影した写真のライセンスは「 `CC-BY <https://creativecommons.org/licenses/by/4.0/deed.ja>`_ を基本とし、本人が写っている物をアイコン等に使用することが自由にできるようにする。」と一般社団法人 PyCon JP で定められています。

- `PyCon JP ライセンスについて <https://www.pycon.jp/committee/license.html>`_

自分たちの撮影した写真をプロフィールなどに設定されるととても嬉しいので、是非 `PyCon JP | Flickr <https://www.flickr.com/photos/pyconjp/>`_ から自分の写真を探してみてください。

アイコンに使えそうな写真が無かったという方には朗報です。スピーカーはもれなく撮影されますよ。来年はプロポーザルを出しましょう！

最後に
=========
執筆担当: メディアチームメンバー
骨子: `SAR-1268 <https://pyconjp.atlassian.net/browse/SAR-1268>`_
