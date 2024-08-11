# SSMAS

## Overview
**SSMAS**: Sequential Structured Multimodal (interleaved image-text) Abstractive Summarization dataset.  
The **SSMAS** dataset is an extension of [**XSum**](https://github.com/EdinburghNLP/XSum), which is built based on [BBC](https://www.bbc.com/news) News.  

## Dataset Description

- **Data Format**: json  
- **Size**: < 1GB  
- **Number of Samples**: 192418  
- **Partitioning**: SSMAS is split according to the XSum dataset [here](https://github.com/EdinburghNLP/XSum/blob/master/XSum-Dataset/XSum-TRAINING-DEV-TEST-SPLIT-90-5-5.json) 

## Structure

The structure of each data sample:

<ul>
    <li>SSMAS</li>
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


## License

The SSMAS dataset is released under the Apache License. Please see the LICENSE file for details.

## Citation

If you use this dataset in your research, please cite it as follows:

```
@InProceedings{
author={Rui He, Minjie Qiang, Hongling Wang, Zhongqing Wang},
title={Sequential Structured Fusion of Image and Text for Enhanced Multimodal Abstractive Summarization},
booktitle={The 13th CCF International Conference on Natural Language Processing and Chinese Computing},
year={2024},
}
```

