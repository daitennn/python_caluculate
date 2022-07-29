# 概要
Numpyを用いて、単回帰分析の最適なパラメータの計算を行った。

# 内容
|$n$|$x_{n}$|$t_{n}$|
|:--|:--|:--|
|1|20|60000|
|2|40|115000|
|3|60|155000|

上記の数値が与えられている中、最適なパラメータである

$$
w = \frac{\sum_{n=1}^N x_n t_n}{\sum_{n=1}^N x^2_n}
$$

を求める。

また、この場合を用いた、x=50の予測値を以下の式に基づいて、計算する。

$$
y = w(x - \bar{x}) + \bar{t}
$$

以上から、求めることができた解を以下に記載。

w = 2375.0

y = 133750.0

よって、Pythonを用いて、機械学習を行うことができた。
