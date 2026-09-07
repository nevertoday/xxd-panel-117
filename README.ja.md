<div align="center">

# XXD Panel 117｜細線淡彩余白誌

一つの視覚の核から、写真の主題と余白を演出し直す。

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <strong>日本語</strong> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## サンプル展示

以下のサンプルはそれぞれ異なる原画像を使い、Panel 117 が一枚ずつ独立した一回の生成で作成しました。AIメタデータは削除済みです。横長は左に実写、右にデザインを置く厳密な50:50、縦長は上に実写、下にデザインを置く厳密な50:50です。

原画像は異なる素材フォルダから選び、各サンプルに内容に即した英語の文言を生成します。

**16:9 横長 · 左右 50:50**

| sample-05 | sample-06 |
|---|---|
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |

**3:4 縦長 · 上下 50:50**

| sample-09 | sample-10 |
|---|---|
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 向いている場面と解決する課題

写真が雑然としていたり構図が平凡でも、残す価値のある何かがあれば、**Panel 117** は一つの核心テーマ、一つの視覚的な核、一つの感情的な関係を抽出し、細線、淡い平塗り、紙の質感、軽いコラージュによる小さな画面へ演出し直します。比較領域に実写を残しながら、意図的な余白でデザインを独立させます。

### こんな場合に

- 原物の識別性を保ち、主体の位置、大きさ、方向、切り取りを再設計したい。
- 物ごとの描き写しや雑然とした背景ではなく、少要素で強い主題を作りたい。
- 写実的な細部や滑らかなベクターより、細線、柔らかなパステル、呼吸する紙面が好き。
- 上下、左右、デザインのみ、複数比率、4端末壁紙、フォルダ一括に対応したい。

### 解決すること

- 複雑な素材から重要な視覚の核を選び、二次情報を削ります。
- 余白が正負の形、距離、非対称の均衡を構成します。
- 比較は各50%の2領域のみとし、第三帯や入れ子のパネルを作りません。
- 出力ごとに現在の原画像から独立した一回の生成を行い、中間結果を再転写しません。

## 原文プロンプト · 5言語

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中国語ファイルは原文を逐字保存し、実行時の唯一の創作・美的権威です。他4言語は完全で忠実な閲覧用翻訳です。左右など既定以外のモードを明示的に選んだ場合、アダプターは位置と寸法だけを変換し、美的要件は変えません。

**特徴語：** 一つの核心テーマ · 一つの視覚の核 · 一つの感情的関係 · 細線手描き · 淡い平塗り · 紙の質感 · 軽いコラージュ · 小さな章印 · 2–4色 · 大きな余白 · 細い手書き文字

## クイック判定

| 気になること | Panel 117 の答え |
|---|---|
| 平凡な写真でも使えるか | 抽出後に主体の大きさ、位置、方向、切り取りを再設計します。 |
| 原物を認識できるか | 代表的な輪郭、流れ、姿勢、視覚の記憶点を保ちます。 |
| 余白は単なる未描画部分か | 描画面積より明らかに大きく、距離と正負の形を積極的に構成します。 |
| サイズを柔軟にしたい | 一般比率、正確なピクセル、4モード、フォルダ一括に対応します。 |

## 写真を作品に変える流れ

```text
一つの主題・核・感情的関係を抽出 → 他を削除 → 大きさ・位置・切り取りを再設計 → 細線と淡い平塗りで再構成 → 淡色面・紙・軽いコラージュを配置 → 大きな余白と少量の手書き文字で完成
```

## 完成品の識別ポイント

- 少数の簡潔な細い輪郭で主体を識別し、内部線は必要最小限にします。
- 薄く穏やかな色面を使い、任意の極淡い主題色面の縁を主体が越えても構いません。
- 章印のような小主体は偏心、端寄せ、浮遊、切り取りが可能で、余白は描画面積を明らかに上回ります。
- 原画像の2–4色を高明度で澄んだ柔らかなパステルにし、ほぼ白い紙に明快な対比を保ちます。
- 主題や感情由来の極少数の記号を一、二筆で表し、実物の複製や穴埋め装飾はしません。
- 主体、動作、感情、記憶、比喩から少量の言葉を生み、細く自然な手書き感で余白に入れます。

## 4つの出力モード

- `top-bottom`：全幅の上下2領域のみ。実写を上、デザインを下に置き、各50%。
- `left-right`：全高の左右2領域のみ。実写を左、デザインを右に置き、各50%。上下構成へ回転しません。
- `design-only`：全画面を Panel 117 のデザイン翻訳にし、写真は見えない参照にします。
- `wallpaper-pack`：スマートフォン、iPad、デスクトップ、時計を端末ごとに生成。`linked` または `independent` を選べます。

モードと比率は複数指定できます。`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5`、正確なピクセルに対応します。文字はプロンプト生成、指定文の逐字使用、なしから選べます。フォルダ入力では各画像を分離して処理し、PNGを一つの新しいタスクフォルダへ置きます。

## はじめに

```bash
git clone https://github.com/nevertoday/xxd-panel-117.git
npx skills add https://github.com/nevertoday/xxd-panel-117 --skill xxd-panel-117
```

インストール後に Agent セッションを再起動し、`$xxd-panel-117` を呼び出します。ユーザー単位の Codex には `--global --agent codex --yes` を追加できます。

```text
/xxd-panel-117 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ja-JP
/xxd-panel-117 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-117 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-117 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完全な実行契約は [SKILL.md](SKILL.md)、実行アダプターは[英語](references/xxd-panel-117-prompt.en.md)／[中国語](references/xxd-panel-117-prompt.zh-CN.md)を参照してください。

<!-- xxd-readme-ads:start -->
## XXD について

XXD は Xiaoxiaodong のブランド名略称です。作成・管理： [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## サポートとメンバーシップ

> **広告表示：** このセクションのQRコードおよび有料会員・サービスのリンクはXXDのプロモーション情報です。スキャンや購入は任意であり、オープンソースの利用には影響しません。


<!-- xxd-panel-command-system:start -->

すべての将軍 Skills は年額 CNY 699 の共通会員特典に含まれ、別途購入は不要です。

| 階級 | Skill | 担当 |
|---|---|---|
| **将軍級** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 利用可能な番号付き Skills の検出、画像・テーマ・用途からの推薦、番号指定の派遣、同一素材の複数スタイル試作、フォルダー画像の一括割り当てと個別派遣。 |
| **兵士級** | `xxd-panel-NNN` | 各番号が固有の原文プロンプトと美学だけを実行し、将軍から渡された一つの仕事を完成させます。 |

<!-- xxd-panel-command-system:end -->

### 知識星球＋会員プロンプトライブラリ＋全将軍 Skills 会員 · 年額 CNY 699

[知識星球](https://wx.zsxq.com/group/15554814142882)、[XXD 会員プロンプトライブラリ](https://vip.xiaoxiaodong.ai/)、全将軍 Skills 会員は同じ会員権です。**一度の年額決済で3つの特典をすべて利用でき、二重の購入は不要です。**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>

---

<div align="center">

## ☕ オープンソースを支援

このプロジェクトが役に立ったら、Buy Me a Coffee から任意で応援していただけます。

<p align="center"><a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Buy Me a Coffee" width="180"></a></p>

</div>
<!-- xxd-readme-ads:end -->

## ライセンス

本プロジェクト（Skill、プロンプト、スクリプト、文書、付属サンプル画像を含む）は **PolyForm Noncommercial License 1.0.0** の下で提供されます。完全な法的条文は [LICENSE](LICENSE)、公式ページは <https://polyformproject.org/licenses/noncommercial/1.0.0> を参照してください。

分かりやすく言うと：

- 個人は学習、研究、実験、テスト、趣味のプロジェクト、私的娯楽に使用できます。慈善団体、教育機関、公的研究・安全・保健機関、環境保護団体、政府機関も使用できます。
- **非商業目的**であれば、使用、複製、変更、派生物の作成、共有が可能です。共有時には本ライセンス（または上記リンク）と、作者が示したすべての `Required Notice:` 文を添付する必要があります。
- 商用製品・サービス、有料納品、アクセス権やライセンスの販売、商業利用につながることが予想される用途には使用できません。商用利用には著作権者から別途書面による許可を得てください。
- 本契約が付与するのは明記された著作権ライセンスと限定的な特許ライセンスだけです。商標、ブランド名、その他明記されていない権利は付与されず、ライセンスを第三者へ再許諾することもできません。
- 書面で違反通知を受けた場合、32 日以内に遵守状態へ戻り、実際の是正措置を取らなければライセンスは直ちに終了します。特許侵害を書面で主張した場合も特許ライセンスが終了します。
- 内容は法律が認める範囲で「現状のまま」提供され、保証はありません。利用に伴うリスクと損失は利用者が負います。
