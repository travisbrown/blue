# Twitter Blue

This repository contains information about [Twitter Blue subscriptions](https://help.twitter.com/en/using-twitter/twitter-blue).

The `data/accounts.csv` file has the following fields:

1. Account ID
2. Screen name
3. Legacy verification status
4. Follower count
5. Date of first identification as Blue subscriber
6. Timestamp of first identification as Blue subscriber
7. Subscription status

The legacy verification status will either be empty (no legacy verification) or one of the following values:

* `B`: verified as a business account
* `G`: verified as a government account
* `V`: verified but verification type is not specified

The subscription status will be one of the following:

* `B`: Subscribed to Twitter Blue
* `U`: Unsubscribed
* `S`: Permanently suspended
* `D`: Self-deactivated

