# reddit-affective-content
Reddit post and comment data for analysis of disclosure and supportiveness discourse.

The dataset is downloaded using [PRAW](https://praw.readthedocs.io/en/latest/).

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

10, 12, 14, 16. are weak labels: 1 - some part of comment is labeled in Affcon dataset and 
                  0 - comment is not labeled at all in Affcon dataset
                  
11, 13, 15, 17. are sentence ids previously labeled in Affcon-2020


tree_info.csv has comment tree information.
The fields are as follows:
1. treeid: id of comment tree
2. max_depth: maximum depth of conversation
3. length: length of the comment tree
