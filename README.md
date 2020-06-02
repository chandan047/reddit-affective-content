# reddit-affective-content
Reddit post and comment data for analysis of disclosure and supportiveness discourse.

The dataset is downloaded using [PRAW](https://praw.readthedocs.io/en/latest/)

forest.csv has all the comments information for the posts from AffCon-2020 dataset. 
The fields are as follows:
1. commentid: id of comment
2. treeid: id of comment tree
3. authors: author of the comment
4. created_utc: comment creation time
5. score: score of comment
6. wordcount: number of words in comment
7. full_text: body of the comment
8. parent: parent comment id, -1 if parent is post
9. postid: id of reddit post

Columns 10, 12, 14, 16, 18, 20. are weak labels: 0/1 - some part of comment is labeled in Affcon dataset and -1 - comment is not labeled at all in Affcon dataset. Columns 11, 13, 15, 17, 19, 21. are ids of sentences previously labeled in Affcon-2020


tree_info.csv has comment tree information.
The fields are as follows:
1. treeid: id of comment tree
2. max_depth: maximum depth of conversation
3. length: length of the comment tree


Number of partially labeled posts 3582. Mean length of partially labeled posts 23.64. Stddev length of partially labeled posts is 44.08. This is in reference to the Affcon 2020 dataset.

![Plot](/plots/1.png)


Number of partially labeled posts with at-least 5 length 2763. Mean length of partially labeled posts with at-least 5 length 29.67. Stddev length of partially labeled posts with at-least 5 length 48.58.

![Plot](/plots/2.png)


Number of partially labeled posts with at-least 10 length 1950. Mean length of partially labeled posts with at-least 10 length 38.77. Stddev length of partially labeled posts with at-least 10 length 55.33.

![Plot](/plots/3.png)


Mean length of all posts 17.04. Stddev length of partially labeled posts 35.02.

![Plot](/plots/4.png)


Mean score of partially labeled posts 163.42. Stddev score of partially labeled posts 784.97.

![Plot](/plots/5.png)


Mean score of all posts 110.67. Stddev score of all posts 632.60.

![Plot](/plots/6.png)
