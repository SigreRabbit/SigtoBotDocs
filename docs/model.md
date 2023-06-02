---
title: "モデルについて"
description: ""
custom_edit_url: null 
sidebar_position: 3
---

# モデルについて

## 説明

モデルは、主に絵柄に影響する

- デフォルトではBNOM（BloodNightOrageMix）が指定される

- まずはALLで絵柄を確認するのがおすすめ

## モデル一覧

|モデル名|イラスト傾向|ファイル名|ソース|
|:--|:--|:--|:--|
|A1_Counterfeit|陰影が強い　顔や背景が特に精細|Counterfeit-V2.5_fp16.safetensors|[Hugging Face](https://huggingface.co/gsdf/Counterfeit-V2.5)|
|A2_BreakDomainAnime|リアル寄りアニメ風　メカや建物に強い||[Civitai](https://civitai.com/models/72675/breakdroidanime)|
|A3_ClossmixSIERRA|やや陰影が強い　年齢低めになる||[Hugging Face](https://huggingface.co/Yashiro/Closs_mix)|
|||||
|B1_BNOM（デフォルト）|強い特徴がなく、高い完成度|||
|B2_Kawaiiniji|繊細な線　珍しい構図が出やすい||[Civitai](https://civitai.com/models/52922/kawaiiniji)|
|B3_El_Dorado|比較的平面的なイラスト|El Dorado.safetensors|[Hugging Face](https://huggingface.co/deadman44/SD_Anime_Merged_Models)|
|||||
|C1_CuteYukiMix|SDとイラストの中間点||[Civitai](https://civitai.com/models/28169/cuteyukimix)|
|C2_KawAICE|かなりSD寄り　淡い色使い|||
|C3_threeAB|はっきりSD　塗りや線が強い|||
|||||
|ALL|モデルだけ変えて9枚生成|||

## その他

- Aは繊細、Bは平均的、CはSDっぽい傾向にしているので、その間でいろいろ試すといい
  
- ALLのときの画像は以下の順<br/>
  A1 A2 A3<br/>
  B1 B2 B3<br/>
  C1 C2 C3

- ALLについては、同じシードで似にくいモデルを選んでいるので、比較にならないこともあるかも

- 他のモデルで試したいのがあれば教えてください
