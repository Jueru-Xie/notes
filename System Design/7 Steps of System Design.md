# 7 Steps of System Design

### 1. Requirment clarfication
Clarifications of requirements, what functions needs to be considered.

### 2. Back-of-the-envelope estimation
Estimate the scale.

### 3. System  interface definition
Define the APIs that are expected from the system.

Example:
postTweet(user_id, tweet_data, tweet_location, user_location, timestamp, …)
markTweetFavorite(user_id, tweet_id, timestamp, …)

### 4. Defining data model
Design the data modeel that will be used by the system.

Example:
User: UserID, Name, Email, DoB...
Tweets: TweetID, Content, Location, TimeStamp, #ofLikes...
UserFollow: UserID1, UserID2...
LikedTweets: UserID, TweetID, TimeStamp...

### 5. High-level design
Use a diagram with boxes to represent the core components. 

### 6. Detailed design
Dig deeper into tw or three major components, following the interviewer's feedback.

Example:
- Since we will be storing a massive amount of data, how should we partition our data to distribute it to multiple databases? Should we try to store all the data of a user on the same database? What issue couldit cause?
- What components need better load balancing?
- How much and at which layer should we introduce cache to speed things up?

### 7. Identifying and resolving bottlenecks
Discuss as many bottlenecks/potential failure as possible.

Example:
- Is there any single point of failure in our system? What are we doing to mitigate it?
- Do we have enough replicas of the data so that if we lose a few servers, we can still serve our users?
- How are we monitoring the performance of our service? Do we get alerts whenever critical components fail or their performance degrades?


