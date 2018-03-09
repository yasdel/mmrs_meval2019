# Datasets

The <b>Audio descriptors</b> folder contains two sub-folders: <a href="http://www.cp.jku.at/people/schedl/Research/Publications/pdf/seyerlehner_smc_2010.pdf" target="_blank">block-level features (BLF)</a> and <a href="http://www.cp.jku.at/people/schedl/Research/Publications/pdf/eghbal-zadeh_ismir_2015.pdf" target="_blank">i-vector features</a>. The BLF contains 6 descriptors computed from the audio spectrum, among others, spectral patterns (modeling the timbral content), fluctuation patterns (modeling the strength of recurring beats over various frequency bands), and correlation patterns (modeling the correlation between frequency bands to uncover harmonic characteristics). The i-vector features describe timbral characteristics of audio by modeling distributions over <a href="http://musicweb.ucsd.edu/~sdubnov/CATbox/Reader/logan00mel.pdf" target="_blank">Mel frequency cepstral coefficients (MFCCs)</a>.

While the BLF data includes the raw features of the 6 subcomponents and similarities computed thereon, the i-vector features include different parameters for the Gaussian mixture model (GMM) and total variability dimension (tvDim). The BLF folder has two subfolders: <i>All</i> and <i>Component6</i>; the former contains the similarities computed using all 6 subcomponents, the latter contains the raw feature vectors of the subcomponents in separate CSV files.

<img src="Audio_folder.jpg" alt="MMTF-14K Audio" height="50%" width="50%">


The <b>Visual descriptors</b> folder contains two subfolders: <a href="https://peerj.com/articles/1390/" target="_blank">Aesthetic features</a> and <a href="https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf" target="_blank">AlexNet features</a>, each of them including different aggregation schemes for the two types of visual features. The Aesthetic features were proposed to measure the aesthetic value of coral reef pictures first and were then used to deal with artwork and photographic aesthetics. The Aesthetic features contain 3 types of descriptors: color based descriptors, texture based descriptors and object based descriptors.





<img src="Visual_features.jpg" alt="MMTF-14K Visual" height="50%" width="50%">

