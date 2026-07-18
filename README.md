
# 計量経済学Basic サポートページ

<!-- badges: start -->
<!-- badges: end -->

**計量経済学Basic** (川田恵介著, 新世社) 用のサポートページです

# RとIDEの整備

- [CRANのホームページ](https://cran.r-project.org/)から, Rをインストールしてください。

- **統合開発環境** (**ID**E; 自動補完やファイル管理など, Rによるデータ分析をサポートするソフト)をインストールしてください。Rについては、いくつかの有力な選択肢があります;

  - **Positron**: Posit社が提供するIDE ([Positのホームページ](https://positron.posit.co/install.html)) です。VS codeをベースに, データや変数の閲覧機能などに優れています。
  
  - 他にも**Rstudio**, **VS code**などもおすすめです

## パッケージの整備

Rに同梱されているinstall.packages関数を用いて、pak パッケージをまずインストールしてください。

``` r
install.packages("pak")
```

pakパッケージには、pak関数が同梱されており、パッケージを安定的にインストールできます。
以下のコードにより、本書の実習に必要なパッケージをインストールしてください;

``` r
pak::pak("tetokawata/data4kawata") # 実習用データ

pak::pak("tidyverse") # データ読み込み/整備/可視化
pak::pak("estimatr") # OLS
pak::pak("gtsummary") # 記述統計
pak::pak("corrr") # 共分散
pak::pak("car") # ブートストラップ
pak::pak("cobalt") # 分布の比較
pak::pak("hdm") # LASSO
pak::pak("sensemakr") # 頑強性分析
pak::pak("fixest") # OLS (sensemakr用)
```
