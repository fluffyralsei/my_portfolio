# my_portfolio
これは私のポートフォリオです

# ゲームシステム分析ポートフォリオ

## 1. 〇〇（ゲーム名）のコアサイクル分析
このゲームの「やめ時を失う仕組み」をエンジニア視点で分析しました。

### コアサイクル図
---
config:
  layout: fixed
---
flowchart TB
    A["Christmas"] -- Get money --> B("Go shopping")
    B --> C{"Let me think"}
    C -- One --> D["Laptop"]
    C -- Two --> E["iPhone"]
    C -- Three --> F["fa:fa-car Car"]
    A --> n1["Untitled Node"]
    n1 --> n2["Untitled Node"]
    n5["Database"] --> n6["Untitled Node"]
    n3["Rectangle"]
    n4["Rounded"]
    n7["Untitled Node"]

    n5@{ shape: db}
    n3@{ shape: rect}
    n4@{ shape: rounded}
    n7@{ shape: rect}
