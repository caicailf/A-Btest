# A-Btest

# 项目说明

理解电子商务网站运营 A/B 测试的结果。通过这个 Notebook，帮助公司理解他们是否应该设计新页面、保留原有网页或延长测试时间以便做出决定。

# 库
<pre><code>import pandas
</code></pre>

<pre><code>import numpy
</code></pre>

<pre><code>import random
</code></pre>

<pre><code>import matplotlib
</code></pre>

<pre><code>import statsmodels
</code></pre>

# 分析方法：

运用假设检验和抽样分布的统计学方法，对新旧页面转化数据进行分析，
#### 零假设为：P（新页面转化率）<= P（旧页面转化率）；备择假设：P（新页面转化率）> P（旧页面转化率）
得出P值偏大，所以我们无法拒绝零假设。最后建立逻辑回归模型，验证检验结果。
