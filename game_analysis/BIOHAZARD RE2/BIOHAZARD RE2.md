# バイオハザード RE2


<img width="1650" height="329" alt="スクリーンショット 2026-04-15 194044" src="https://github.com/user-attachments/assets/a85ece9c-472d-46fb-8b55-8a1624dd3269" />


## ゲーム概要、選定理由
### ゲーム概要

全てがプレイヤーの想像を裏切り上回る。\
1998年9月にラクーンシティを襲った生物災害。ゾンビが生者を引き裂く地獄から生還せよ。 \
<span>(steamstoreページより)</span>

### 選定理由
私が初めてクリアしたホラーゲームだから。\
他のゲームジャンルでは得られない楽しさを感じたため。\


## 分析の流れ
### 1.ゲームループ
ループ図解...このゲームがどんな行動を繰り返すか\
おもしろさのポイント


## 分析
### 1.ゲームループ
### ループ図解
```mermaid
---
config:
  theme: neutral
---
flowchart TD
    %% ノードの定義
    A["探索フェーズ<br/>扉の確認・未知のエリア探索・アイテム探し"]
    B["発見フェーズ<br/>敵・障害・謎解きとの遭遇"]
    C["判断フェーズ<br/>戦闘・逃走・アイテム使用"]
    D["収穫フェーズ<br/>報酬獲得・新エリアの解禁"]

    %% 流れの定義
    A -->|"発見"| B
    B -->|"意思決定"| C
    C -->|"実行・解決"| D
    D -->|"次のステージへ"| A

    %% スタイルの調整
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style C fill:#fb1,stroke:#333,stroke-width:2px
    style D fill:#9f9,stroke:#333,stroke-width:2px
```
バイオハザードRE2のゲームループは探索、遭遇、判断、収穫の4つのフェーズで構成される。\
このループが「極限サバイバル体験」を実現している

##おもしろさのポイント
このゲームの面白さを設計の観点から考察していく

### リソース不足設計
バイオハザードRE2の面白さの一つ目は圧倒的なリソース不足設計です。
ここで言う「リソース」とは銃を撃つために必要な銃弾やハーブ(回復薬)などの必須アイテム、インベントリの上限のことを指しています
<br>
<br>

<img width="1920" height="1080" alt="883710_38" src="https://github.com/user-attachments/assets/83840bd5-e123-4439-9704-d3c63d8c65f3" />

例えば、このゲームの銃弾はかなり少ない量しか入手できないようになっています。
この設定がプレイヤーの行動に迷いを発生させています。
```mermaid
---
config:
  theme: neutral
---
flowchart TB
    A["敵に遭遇!"] -- 逃げる？ --> B["弾丸を節約!"]
    A -- 倒す？ --> C["不安要素除去！"]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style C fill:#fb1,stroke:#333,stroke-width:2px
```



リソースを消費して不安から解放されるか、リスクの上で逃げることを選ぶか、この判断をさせることこそが面白さの要因




### 邪魔なゾンビ









