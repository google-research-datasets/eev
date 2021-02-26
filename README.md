# Evoked Expressions in Video (EEV) Dataset

Videos can evoke a range of affective responses in viewers. The ability to predict evoked affect from a video, before viewers watch the video, can help in content creation and video recommendation. We introduce the Evoked Expressions from Videos (EEV) dataset, a large-scale dataset for studying viewer responses to videos. Each video is annotated at 6 Hz with 15 continuous evoked expression labels, corresponding to the facial expression of viewers who reacted to the video. We use an expression recognition model within our data collection framework to achieve scalability. In total, there are 8 million annotations of viewer facial reactions to 5,153 videos (370 hours). We use YouTube to obtain a diverse set of video content. We hope that the size and diversity of the EEV dataset will encourage further explorations in video understanding and affective computing.

## Structure of the Dataset

The datset consists of two files, train.csv and val.csv, that represent the training and validation splits respectively. We are not releasing the test split at this time. Each CSV file contains the expected facial expressions of someone reacting to a specific content video. Each line indicates a specific YouTube video represented by its video ID, a timestamp in milliseconds, and a set of expression scores. The first line of the CSV is a header with the labels for each column. The reaction annotations are sampled at 6 frames per second such that there could be thousands of lines for a single YouTube video.

## Dataset Over Time

Because this dataset is from YouTube videos. There may be instances where specific videos are no longer available on the platform and those annotations will be removed from the dataset. This means there is a possibility that the dataset may decrease in size over time.

## How to Cite the Dataset

Please consider citing our [paper](https://arxiv.org/abs/2001.05488) if you find the dataset useful:

```
@article{sun2021eev,
      title={EEV: A Large-Scale Dataset for Studying Evoked Expressions from Video}, 
      author={Sun, Jennifer J and Liu, Ting and Cowen, Alan S and Schroff, Florian and Adam, Hartwig and Prasad, Gautam},
      year={2021},
      journal={arXiv preprint arXiv:2001.05488}
}
```
## License

This data is licensed by Google LLC under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). Users will be allowed to modify and repost it, and we encourage them to analyze and publish research based on the data.

## Contact Us

If you have a technical question regarding the dataset, code or publication, please create an issue in this repository. You may also reach us at eev-dataset@google.com.
