# Tweets Collection Python + Mysql

By Using Python3 and Mysql WorKbench, we can collect and store tweets data, all tweets will stored by ID to avoid data duplication.
Firstly, you must install some requirements:
1. install GetOldTweets3 library  from : https://pypi.org/project/GetOldTweets3/
2. install pymysql library
3. install mysql-connector library
4. install Mysql WorKbench: https://www.sqlshack.com/how-to-install-mysql-database-server-8-0-19-on-windows-10/


##  Create Table under database called : tweetsdb
CREATE TABLE `tweetsuniv` (
  `tweetID` varchar(255) NOT NULL,
  `track` varchar(255) DEFAULT NULL,
  `user` varchar(100) DEFAULT NULL,
  `created_at` varchar(100) DEFAULT NULL,
  `towho` varchar(255) DEFAULT NULL,
  `tweet` text,
  `hashtags` text,
  `mentions` varchar(255) DEFAULT NULL,
  `retweet_count` int DEFAULT NULL,
  `likes` int DEFAULT NULL,
  PRIMARY KEY (`tweetID`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
