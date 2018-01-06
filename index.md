# Movie Trailers Rich Multimedia Dataset

| [Home](index.md) | [Datasets](datasets.md) | [Benchmark](benchmark.md) | [v1.0](version.md) | [Community](community.md) |

TEMPORARY SKELETON TAKEN FROM Visual Tracker Benchmark

## Introduction

This website contains data and code of the benchmark evaluation of online visual tracking algorithms.
Join visual-tracking Google groups for further updates, discussions, or QnAs.

You can find the following resources from this site.
- Benchmark results
- Dataset with ground-truth annotations
- Code library

Later we have plan to add
- Online submission script that facilitates evaluating your algorithms.

## Tracker Results used in the PAMI15 paper

The raw results (zipped matlab .mat files) can be downloaded at the following links.
- v1.1/pami15_SRE.zip (250,651,768 bytes) : SRE results for the baseline trackers.
- v1.1/pami15_TRE.zip (223,347,083 bytes) : TRE results for the baseline trackers.
- v1.1/pami15_SRER.zip (1,037,508,658 bytes) : SRER results for the baseline trackers.
- v1.1/pami15_SRE_rev.zip (56,328,515 bytes) : SRE results for more recent trackers.
- v1.1/pami15_TRE_rev.zip (38,265,788 bytes) : TRE results for more recent trackers.

## How to get the tracker benchmark codebase.

The tracker codes used in this benchmark can be download: tracker_benchmark_v1.0.zip (229MB).
If you suffer from slow download speed, try this file on Google Drive.
The benchmark results using the above code is available also : tracker_benchmark_v1.0_results.zip (222MB, or Google Drive version).
The results zip-file needs to be unzipped in the ‘tracker_behcnmark_v1.0′ directory.
- We are building a new Python-based test suite https://github.com/jwlim/tracker_benchmark.

## How to get the test data.

Simply, you can download the test sequence from the link in the test sequences table. For evaluating your tracker, you can find the ground-truth markings as well as MATLAB functions for evaluation in the the benchmark codebase.

## How to compare your result with the benchmark results.

The benchmark results are reported as success plots and precision plots. Note that the reported performance is the average over all sequences in the category. The test sequences table and attributes table shows which sequence has which attributes. For the detailed information about evaluation, refer the CVPR 2013 paper above.

Consider the performance of each tracker reported in this site as a reasonable lower-bound performance. We used one default parameter (used in the original implementation) for all sequences without any tuning. In later versions the performance of the trackers may be updated. However, we still do NOT allow hand-tuning and using different parameters for individual sequences.

The **protocol for tracker evaluation** using the benchmark data:
- Tracking starts from one initial bounding box in a start frame.
    The start frame may not be the first frame of the sequence.
- DO NOT use manually-tuned, different parameters for individual sequences.
- Any additional information, such as sequence name or attributes, may not be used in determining the parameters.
- It is allowed for a tracker to automatically adapt its parameters only using features from input images.
- The tracking result is a sequence of bounding boxes at each frame.
- Affine or similarity parameters are converted into bounding boxes for comparison.
- Use the AUC (area under curve) to show the tracker’s overall performance.
- The success plots are preferred over the precision plots, since precision only uses the bounding box locations, and ignores the size or overlap.







FOO

Hyashar yashar yashar yashar yashar
## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/mmprj/mtrm_dataset/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/mmprj/mtrm_dataset/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
