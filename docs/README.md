# SVQA2：A Benchmark for spatial-temporal reasoning of video question answering 



# SVQA-synthetic

## Introduction

Video question answering (VideoQA) always involves visual reasoning. When answering questions composing of multiple logic correlations, models need to perform **multi-step reasoning**. [SVQAv1]() (Synthetic Video Question Answering) formulate multi-step reasoning in VideoQA as a new task to answer compositional and logical structured questions based on video content. Compared with other VideoQA datasets, SVQA contains exclusively long and structured questions with various spatial and temporal relations between objects. More importantly, questions in SVQA can be decomposed into human readable logical tree or chain layouts, each node of which represents a sub-task requiring a reasoning operation such as comparison or arithmetic. 



## Dataset

The SVQA(Synthetic Video Question Answering) dataset contains 39,745 videos and around 350k QA pairs. Videos and QA pairs are all generated automatically with minimal language biases and clearly defined question categories. The dataset can facilitate the analysis on models reasoning skills.

You can download the dataset from this [link](https://pan.baidu.com/s/1ggyv0CwRBSXs-2dj3GJ3aw?pwd=wr5d ).


### Video and QA Pair Examples

| QA Category          | Question                                         | Answer | Video(GIF)        |
| :------------------- | ------------------------------------------------ | ------ | ----------------- |
| Attribute Comparison | <img width="1200" src="GIF/6.jpg"/>              | no     | ![](GIF/3997.gif) |
| Count                | <img width="1200" src="GIF/7.jpg"/>              | 5      | ![](GIF/377.gif)  |
| Query                | <img width="1200" src="GIF/8.jpg"/>              | blue   | ![](GIF/1792.gif) |
| Integer Comparison   | <img width="1200" height="120" src="GIF/9.jpg"/> | no     | ![](GIF/4929.gif) |
| Exist                | <img width="1200" src="GIF/10.jpg"/>             | yes    | ![](GIF/6517.gif) |

## Statistics of SVQA

<!-- | Question  Category           | Sub  Category | QA_pairs2 | QA_pairs1 |
| ---------------------------- | ------------- | --------- | --------- |
| Count                        |               | 27600     |            |
| Exist                        |               | 9600      |            |
| Query & Attribute Comparison | Color         | 14232     | 99442     |
|                              | Size          | 14232     | 83619     |
|                              | Action Type   | 13032     | 83619     |
|                              | Direction     | 14232     | 95188     |
|                              | Shape         | 14232     | 97332     |
| Integer Comparison           | More          | 3840      |           |
|                              | Equal         | 3840      |           |
|                              | Less          | 3840      |           |
| Total QA pairs               |               | 118800    | 472829    |
| Total Videos                 |               | 12000     | 27745     | -->

| Question  Category           | Sub  Category | QA_pairs2 | QA_pairs1 |
| ---------------------------- | ------------- | --------- | --------- |
| Count                        |               | 27600     |            |
| Exist                        |               | 9600      |            |
| Query & Attribute Comparison | Color         | 14232     | 74204     |
|                              | Size          | 14232     | 62397     |
|                              | Action Type   | 13032     | 62397     |
|                              | Direction     | 14232     | 71030     |
|                              | Shape         | 14232     | 72629     |
| Integer Comparison           | More          | 3840      |           |
|                              | Equal         | 3840      |           |
|                              | Less          | 3840      |           |
| Total QA pairs               |               | 118800    | 459200    |
| Total Videos                 |               | 12000     | 27745     |

# SVQA-real

In addition, we automatically generated a supplementary dataset based on the [something-something v2](https://developer.qualcomm.com/software/ai-datasets/something-something) dataset to test the model's spatio-temporal reasoning ability in the real world. This dataset contains **71,075 videos** and **341,044** different types of question and answer pairs, which can be downloaded at [this link](https://pan.baidu.com/s/1Bsz5TCaeAuySoa9imqHz1A?pwd=kxgp ).

