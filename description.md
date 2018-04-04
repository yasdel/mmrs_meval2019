# Description

The <b>Audio descriptors</b> consist of two classes of descriptors: <a href="http://www.cp.jku.at/people/schedl/Research/Publications/pdf/seyerlehner_smc_2010.pdf" target="_blank">block-level features (BLF)</a> and <a href="http://www.cp.jku.at/people/schedl/Research/Publications/pdf/eghbal-zadeh_ismir_2015.pdf" target="_blank">i-vector features</a>. The BLF contains 6 descriptors computed from the audio spectrum, among others, spectral patterns (modeling the timbral content), fluctuation patterns (modeling the strength of recurring beats over various frequency bands), and correlation patterns (modeling the correlation between frequency bands to uncover harmonic characteristics). The i-vector features describe timbral characteristics of audio by modeling distributions over <a href="http://musicweb.ucsd.edu/~sdubnov/CATbox/Reader/logan00mel.pdf" target="_blank">Mel frequency cepstral coefficients (MFCCs)</a>.

The <b>Visual descriptors</b> also consist of two categories of descriptors: <a href="https://peerj.com/articles/1390/" target="_blank">Aesthetic features</a> and <a href="https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf" target="_blank">AlexNet features</a>, each of them including different aggregation schemes for the two types of visual features. The Aesthetic features were proposed to measure the aesthetic value of coral reef pictures first and were then used to deal with artwork and photographic aesthetics. The Aesthetic features contain 3 types of descriptors: color based descriptors, texture based descriptors and object based descriptors. AlexNet deep neural network has been developed for scene and object recognition tasks. In our context, we use the extracted output values of the fc7 layer.






