# SVQA2：A Benchmark for spatial-temporal reasoning of video question answering 



# SVQAv1 

## Introduction

Video question answering (VideoQA) always involves visual reasoning. When answering questions composing of multiple logic correlations, models need to perform **multi-step reasoning**. [SVQAv1]() (Synthetic Video Question Answering) formulate multi-step reasoning in VideoQA as a new task to answer compositional and logical structured questions based on video content. Compared with other VideoQA datasets, SVQA contains exclusively long and structured questions with various spatial and temporal relations between objects. More importantly, questions in SVQA can be decomposed into human readable logical tree or chain layouts, each node of which represents a sub-task requiring a reasoning operation such as comparison or arithmetic. 



## Dataset

The SVQA(Synthetic Video Question Answering) dataset contains 31,690 videos and around 600k QA pairs. Videos and QA pairs are all generated automatically with minimal language biases and clearly defined question categories. The dataset can facilitate the analysis on models reasoning skills.



### Video and QA Pair Examples

| QA Category|Question|Answer|Video(GIF)

| :----------------- | --------------------------------- | ----------------------------- | ---------------------------------------- |
| ------------------ | --------------------------------- | ----------------------------- | ---------------------------------------- |
|                    |                                   |                               |                                          |
| Attribute Comparison | <img width="1200" src="GIF/6.jpg"/> | no   | ![](GIF/3997.gif) |
| -------------------- | ----------------------------------- | ---- | ----------------- |
|                      |                                     |      |                   |
| Count | <img width="1200" src="GIF/7.jpg"/> | 5    | ![](GIF/377.gif) |
| ----- | ----------------------------------- | ---- | ---------------- |
|       |                                     |      |                  |
| Query | <img width="1200" src="GIF/8.jpg"/> | blue | ![](GIF/1792.gif) |
| ----- | ----------------------------------- | ---- | ----------------- |
|       |                                     |      |                   |
| Integer Comparison | <img width="1200" height="120" src="GIF/9.jpg"/> | no   | ![](GIF/4929.gif) |
| ------------------ | ------------------------------------------------ | ---- | ----------------- |
|                    |                                                  |      |                   |
| Exist | <img width="1200" src="GIF/10.jpg"/> | yes  | ![](GIF/6517.gif) |
| ----- | ------------------------------------ | ---- | ----------------- |
|       |                                      |      |                   |



## Statistics of SVQA
| Question Category        | Sub Category | Train |   Val |  Test |
| :----------------------- | :----------- | ----: | ----: | ----: |
| **Count**                |              | 19320 |  2760 |  5520 |
| **Exist**                |              |  6720 |   960 |  1920 |
| **Query**                | Color        |  7560 |  1056 |  2160 |
|                          | Size         |  7560 |  1056 |  2160 |
|                          | Action Type  |  6720 |   936 |  1920 |
|                          | Direction    |  7560 |  1056 |  2160 |
|                          | Shape        |  7560 |  1056 |  2160 |
| **Integer Comparison**   | More         |  2520 |   600 |   720 |
|                          | Equal        |  2520 |   600 |   720 |
|                          | Less         |  2520 |   600 |   720 |
| **Attribute Comparison** | Color        |  2520 |   216 |   720 |
|                          | Size         |  2520 |   216 |   720 |
|                          | Action Type  |  2520 |   216 |   720 |
|                          | Direction    |  2520 |   216 |   720 |
|                          | Shape        |  2520 |   216 |   720 |
| **Total QA pairs**       |              | 83160 | 11880 | 23760 |
| **Total Videos**         |              |  8400 |  1200 |  2400 |