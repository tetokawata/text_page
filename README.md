
# 計量経済学Basic サポートページ

<!-- badges: start -->
<!-- badges: end -->

計量経済学Basic (新世社, 川田恵介著) 用のサポートページです

## パッケージの整備

Rに同梱されているinstall.packages関数を用いて、pak パッケージをまずインストールしてください。

```
install.packages("pak")
```

pakパッケージには、pak関数が同梱されており、パッケージを安定的にインストールできます。
以下のコードにより、本書の実習に必要なパッケージをインストールしてください;

```
pak::pak("tetokawata/data4kawata") # 実習用データ

pak::pak("tidyverse")
pak::pak("estimatr")
pak::pak("gtsummary")
pak::pak("cobalt")
pak::pak("fixest")
pak::pak("hdm")
pak::pak("sensemakr")
```
