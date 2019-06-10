# DataMiningChallenge2018
### Challenge Description 

Reddit is an entertainment, social networking, and news website where registered community members can submit content, such as text posts or direct links, making it essentially an online bulletin board system. Registered users can then vote submissions up or down to organize the posts and determine their position on the site's pages. Content entries are organized by areas of interest called "subreddits". The subreddit topics include news, gaming, movies, music, books, fitness, food, and photosharing, among many others.

When items (links or text posts) are submitted to a subreddit, users (redditors) can vote for or against them (upvote/downvote). Each subreddit has a front page that shows newer submissions that have been rated highly. Redditors can also post comments about the submission, and respond back and forth in a conversation-tree of comments; the comments themselves can also be upvoted and downvoted. The front page of the site itself shows a combination of the highest-rated posts out of all the subreddits a user is subscribed to.

The Reddit website has an API and its code is open source. In July 2015, a Reddit user identified as Stuck_In_the_Matrix made public a dataset of Reddit comments for research. The dataset has approximately 1.7 billion comments and takes 250 GB compressed. Each entry contains comment, score, author, subreddit, position in comment tree and other fields that are available through Reddit's API.

One of the user attributes that is not natively supported by the Reddit platform is the gender. However, in some subreddits, users can self report their genders as part of the subreddit rules. In the scope of this competition, users that self reported their gender are selected from the dataset, and your goal is to predict the gender of these users.

### Evaluation 

The evaluation metric for this competition is the Area Under the ROC Curve. This metric is used to evaluate binary classification, and in the scope of this competition we are representing the gender of the users as binary classes: the class "female" is represented as 1 and the class "male" as 0. The class prediction for each Reddit author corresponds to your confidence that the author is a female, which is a "score" computed for the author (e.g. estimated probability in logistic regression).


### Overview 

We've developed Tf-Idf and Word2Vec approach in order to classify Comments and a simple sparse matrix approach to Author+Subreddit combinations.
