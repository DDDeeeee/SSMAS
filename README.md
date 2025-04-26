# SSMAS

## Overview
**SSMAS**: Sequential Structured Multimodal (interleaved image-text) Abstractive Summarization  
The **SSMSum** dataset is an extension of [**XSum**](https://github.com/EdinburghNLP/XSum), which is built based on [BBC](https://www.bbc.com/news) News.  

<img src="https://github.com/DDDeeeee/SSMAS/blob/main/SSMAS.jpg" alt="Excluding title and first sentence (summary)" style="zoom:25%;" />


## Dataset Description

- **Data Format**: json  
- **Size**: ≈ 25GB  
- **Number of Samples**: 192418  
- **Partitioning**: SSMAS is split according to the XSum dataset [here](https://github.com/EdinburghNLP/XSum/blob/master/XSum-Dataset/XSum-TRAINING-DEV-TEST-SPLIT-90-5-5.json)

## Structure

The structure of each data sample:

<ul>
    <li>SSMSum</li>
    <ul>
        <li>url</li>
        <li>title</li>
        <li>first (summary)</li>
        <li>sent (news text)</li>
        <ul>
            <li>every sentence</li>
        </ul>
        <li>caps</li>
        <ul>
            <li>image caption</li>
            <li>image title</li>
            <li>image url (where you can download the image)</li>
            <li>previous sentence index</li>
            <li>next sentence index</li>
        </ul>
        <li>cap_index (position for inserting caption)</li>
        <li>cap_sent (caption + image title)</li>
        <li>pic_index (position for inserting image, after caption)</li>
    </ul>
</ul>

## Download  

[Baidu Netdisk Download](https://pan.baidu.com/s/1sccjD5waAxcrBVnv5B0S5Q?pwd=47wl), [Google Drive](https://drive.google.com/file/d/1jZMUh6ytKc-1dG08oT5nIXg2nd2faojF/view?usp=drive_link)

## License

The SSMAS dataset is released under the Apache License. Please see the LICENSE file for details.

## Citation
`@inproceedings{he2024sequential,
  title={Sequential Structured Fusion of Image and Text for Enhanced Multimodal Abstractive Summarization},
  author={He, Rui and Qiang, Minjie and Wang, Hongling and Wang, Zhongqing},
  booktitle={CCF International Conference on Natural Language Processing and Chinese Computing},
  pages={290--302},
  year={2024},
  organization={Springer}
}`
