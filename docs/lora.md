---
title: "LoRAについて"
description: ""
custom_edit_url: null 
sidebar_position: 4
---

# LoRAについて

## 説明

promptに入れることで、特定キャラクターに（かなり）近づけたり、絵の傾向に影響を与えたりできる

- 複数のプロンプトワードの影響をまとめた感じ

## 使い方

promptのどこでもいいので、以下の形式で記入する

```<lora:LoRAの名前:強さ>```

- 強さは、正に増やすと影響が強まり、負に増やすと逆の影響が強まる

  - 基本、0.5とか0.25刻みで、2～-2くらいで調整する

  - モデルによって影響力が変わることもある（特にキャラ系）

- 使用例 -> ```1girl, school uniform, <lora:flat2:-1>```

  - ない場合と比較して、服の陰影や髪の書き込みが複雑になるはず
  
- 基本は以下の表からコマンドをコピペでOK
  
  - トリガーワードがあるものは、一緒にコピペする

  - 推奨値があるものはあらかじめそれに合わせている

  - 使用例 -> ```1girl, <lora:KafuuChinoV1:1>, chinokafuu```

## 導入済みLoRA一覧

- 追加したいものがあればお伝えください

  - [Civitai](https://civitai.com) でキャラ名英語で検索して、画像左上に「LORA」って書いてあったらそれ

- たまに全然違う名前がついてるけど、気にせずコピペして

|影響範囲|プラス時の影響( / あればマイナス時の影響)|コマンド(+トリガーワード)|
|:--|:--|:--|
|全体|影などの書き込みが減る / 書き込みが増える|```<lora:flat2:1>,```|
||背景の書き込みが減る / 書き込みが増える|```<lora:flatBG:1>,``` |
||線が太くなる / 線が細くなる|```<lora:boldline:1>,```|
||線がなくなる / 線が増えて太くなる|```<lora:noline:1>,```|
||縁取り線がつく / 線が消える|```<lora:outline:1>,```|
||明るくなる / 暗くなる|```<lora:lit:0.9>,```|
||彩度が上がる / 彩度が下がる|```<lora:saturation:1>,```|
||||
|塗り|アニメ塗りになる|```<lora:anmnr:0.8>, anmnr,```|
||青系で透明感ある絵になる|```<lora:Water:1>,```|
||水彩画風になる|```<lora:Watercolor:1>, watercolor,```|
||厚塗り風になる|```<lora:impasto painting:1>, impasto painting,```|
||輪郭で塗りつぶした画像になる|```<lora:minimalist:1>, anime minimalist,```|
||||
|構図|雑誌の表紙風になる|```<lora:cover:1>, cover,```|
||ポスター風になる|```<lora:Poster painting:1>, Masterpiece, poster design,```|
||背景付き立ち絵になる|```<lora:tachi-e:1>, white background, full body,```|
||黒板に書いた絵になる|```<lora:blackboard:1>, chalkboard, chalk outline,```<br/>(以下必要に応じて) ```traditional media, monochrome,```|
||||
|顔|あごが丸くなる / あごが尖る|```<lora:agomaru:1>,```|
||目が大きくなる / 目が小さくなる|```<lora:bigeye:1>,```|
||顔が幼くなる / 大人寄りになる|```<lora:faceage:1>,```|
||頬が赤くなる / 赤みが少なくなる|```<lora:hohoaka:1>,```|
||しいたけ目になる|```<lora:siitake-eye:1>,```|
||瞳孔が開いた目になる|```<lora:Crazy_ExpressionsV2:1>,```<br/>+ 感情を指定 ```crazy face,``` (狂気), ```scared,``` (怯え)|
||いろいろな目になる|```<lora:moreExpressions:1>,``` + 以下いずれか<br/>```>_<,``` ```@_@``` ```=_=, closed eyes,``` ```X X,``` ```:Ɪ, pout,``` ```._.,``` ```Jitome,```|
||||
|特殊|かっこよく光る|```<lora:GlowingRunesAI:1>, GlowingRunesAI_red,```<br/>```<lora:GlowingRunesAI:1>, GlowingRunesAI_paleblue,```<br/>```<lora:GlowingRunesAI:1>, GlowingRunesAI_green,```<br/>```<lora:GlowingRunesAI:1>, GlowingRunesAI_purple,```<br/>```<lora:GlowingRunesAI:1>, GlowingRunesAI_yellow,```<br/>```<lora:GlowingRunesAI:1>, GlowingRunesAI_pink,```|
||ねんどろいど化する|```<lora:blindbox_v1_mix:1>, chibi, full body,```|
||メカボディになる|```<lora:MechaGirl:1>, mechanical parts,```|
||片目から炎|```<lora:FlamingEye:1>, flaming eye, eye trail,```|
||かっこいい闇と光 ※Hirezfix推奨|```<lora:DarkandLight:1>,```|
||かっこいい日差しと影 ※Hirezfix推奨|```<lora:SunandShadow:1>,```|
||白い板を持つ ※合成とかに使う|```<lora:sign2:1>, Holding_Sign,```|
||きぐるみ的な何かになる|```<lora:fufu3d:1>, wanju\(fufu\),```<br/>※場合により強さ1.1以上に上げる|
||動物が丸っこくなる|```<lora:cute00d_v1:1>, cute00d,``` + animalまたは動物の名前等|
||||
|キャラクター|チノちゃんになる|```<lora:KafuuChinoV1:1>, chinokafuu,```|
||銀狼になる|```<lora:Sv5:1>, SilverWolfV5,```|
||Among Usになる|```<lora:amongus:0.8>, amongus,```|
||マキマさんになる|```<lora:MakimaTestV1:1>, makima \(chainsaw man\),```|
