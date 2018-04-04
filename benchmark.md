# Benchmark
 The primary scope of this dataset is to support the development of movie recommender systems, and this is the first large-scale dataset in the recommender systems community that provides all types of precomputed content-based descriptors in conjunction with metadata in numerical feature format. Part of these data is used in the  <a href="http://www.multimediaeval.org/mediaeval2018/index.html" target="_blank">MediaEval 2018 </a> (task name: "Recommending Movies Using Content: Which content is key?")
 
Through our experiments we aim to provide some baseline results to further help researchers use this dataset and compare their results with other papers and experiments.  We performed extensive experiments to identify the best performing descriptor in unimodal and multimodal settings where for the latter we used the late fusion scheme based on <a href="https://dl.acm.org/citation.cfm?id=1864733" target="_blank">Borda count </a> using a proposed linear weighing scheme which showed to significantly improve the performance of the hybrid approach. 

The competing descriptors are: BLF and i-vector features for audio, AVF and AlexNet Deep features for visual and genre label together with user-generated tags for metadata (baseline).  All the experiments were carried out on a selection of ML-20m rating dataset by random selection of 3000 users each having minimum of 50 ratings associated to the consumption profile. The results are reported based on the average performance in a 5-fold cross validation setup.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-s6z2{text-align:center}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
  <caption> <font size="2"> Table: The best performing descriptor or combination of descriptors with respect to mean reciprocal rank (MRR), mean average precision (MAP), and recall (R) at two cutoff values (@4 and @10)</font> </caption>
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
    <td class="tg-baqh">0.0052</td>
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