# reddit-affective-content
Reddit post and comment data for analysis of disclosure and supportiveness discourse.

forest.csv has all the comments information for the posts from AffCon-2020 dataset. 
The fields are as follows:
commentid: id of comment
treeid: id of comment tree
authors: author of the comment
created_utc: comment creation time
score: score of comment
wordcount: number of words in comment
full_text: body of the comment
parent: parent comment id, -1 if parent is post
postid: id of reddit post
weak_labeled: 1 - some part of comment is labeled in Affcon dataset
              0 - comment is not labeled at all in Affcon dataset


tree_info.csv has comment tree information.
The fields are as follows:
treeid: id of comment tree
max_depth: maximum depth of conversation
length: length of the comment tree
