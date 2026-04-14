# my_portfolio
これは私のポートフォリオです




## 『ポケットモンスター』シリーズのゲームループ分析

ポケモンの面白さは、「育成」と「収集」の2つのループが、「対戦（試行）」を軸に密接に絡み合っている点にあります。

### ゲームループ全体図

```mermaid
graph TD
    %% メインループ（育成と冒険）
    Start((冒険の開始)) --> Battle[野生・トレーナーとの戦闘]
    Battle --> Reward[経験値・賞金の獲得]
    Reward --> Growth[ポケモンのレベルアップ・進化]
    Growth --> Challenge{より強い相手への挑戦}
    Challenge -->|ジムリーダー・四天王| Battle
    
    %% サブループ（収集と編成）
    Battle --> Catch[ポケモンの捕獲]
    Catch --> Collection[図鑑完成・パーティ編成の多様化]
    Collection --> Strategy[タイプ相性を考えた戦略構築]
    Strategy --> Challenge

    subgraph 育成ループ
    Battle
    Reward
    Growth
    end

    subgraph 収集ループ
    Catch
    Collection
    Strategy
    end
