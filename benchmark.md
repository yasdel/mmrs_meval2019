# Benchmark
Through our experiments we aim to provide some baseline results to further help researchers use this dataset and compare their results with other papers and experiments.

The results we will present are obtained through the random selection of 3000 users, with the single condition of each user having more than 50 ratings associated to their profile. We performed a 5 fold cross validation experiment and computed the output values for three related metrics at two cutoff values (@4 and @10):
Mean Reciprocal Rank
Mean Average Precision
Recall

We present the best performing features in the table below, along with the best performing multimodal late fusion scheme (developed by using Borda count):

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-s6z2{text-align:center}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-s6z2"></th>
    <th class="tg-amwm">MRR@4</th>
    <th class="tg-amwm">MAP@4</th>
    <th class="tg-amwm">R@4</th>
    <th class="tg-amwm">MRR@10</th>
    <th class="tg-amwm">MAP@10</th>
    <th class="tg-amwm">R@10</th>
  </tr>
  <tr>
    <td class="tg-amwm">Best unimodal value</td>
    <td class="tg-baqh">0.0233</td>
    <td class="tg-baqh">0.0060</td>
    <td class="tg-baqh">0.0060</td>
    <td class="tg-baqh">0.0311</td>
    <td class="tg-baqh">0.0042</td>
    <td class="tg-baqh">0.0120</td>
  </tr>
  <tr>
    <td class="tg-amwm">Best unimodal feature</td>
    <td class="tg-baqh">i-vec</td>
    <td class="tg-baqh">i-vec</td>
    <td class="tg-baqh">i-vec</td>
    <td class="tg-baqh">i-vec</td>
    <td class="tg-baqh">i-vec</td>
    <td class="tg-baqh">i-vec</td>
  </tr>
  <tr>
    <td class="tg-amwm">Best multimodal value</td>
    <td class="tg-baqh">0.0266</td>
    <td class="tg-baqh">0.0072</td>
    <td class="tg-baqh">0.0059</td>
    <td class="tg-baqh">0.0359</td>
    <td class="tg-baqh">0.0049</td>
    <td class="tg-baqh">0.0139</td>
  </tr>
  <tr>
    <td class="tg-amwm">Best multimodal feature</td>
    <td class="tg-baqh">i-vec+tag</td>
    <td class="tg-baqh">i-vec+tag</td>
    <td class="tg-baqh">i-vec+tag</td>
    <td class="tg-baqh">i-vec+tag</td>
    <td class="tg-baqh">i-vec+tag</td>
    <td class="tg-baqh">i-vec+tag</td>
  </tr>
</table>