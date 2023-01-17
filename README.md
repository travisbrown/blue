# Twitter Blue

This repository contains information about [Twitter Blue subscriptions](https://help.twitter.com/en/using-twitter/twitter-blue).

## About this project

This repository is a continuation of a data collection project started by [Casey Ho](https://twitter.com/CaseyHo) and me ([Travis Brown](https://twitter.com/travisbrown))
in November 2022.

Twitter Blue was first launched on 5 November 2022, and had stopped accepting subscriptions
by 11 November.
The Washington Post [reported](https://www.washingtonpost.com/technology/2022/11/16/musk-twitter-email-ultimatum-termination/) the following week that
"about 150,000 users" had subscribed to the new Twitter Blue during those initial few days, based on information from an internal source.

We eventually identified 145,454 of those initial subscribers, building on an earlier list of 135k we had compiled that was
[reviewed and verified](https://www.washingtonpost.com/technology/2022/11/16/musk-twitter-email-ultimatum-termination/) by the Washington Post.
This work was also cited in the [New York Times](https://www.nytimes.com/interactive/2022/11/23/technology/twitter-elon-musk-twitter-blue-check-verification.html),
[Business Insider](https://www.businessinsider.com/an-estimated-140000-people-paid-twitter-blue-5-days-report-2022-11),
and the SPLC's [Hatewatch](https://www.splcenter.org/hatewatch/2022/11/16/twitter-blesses-extremists-paid-blue-checks).

## Methodology

We compiled this list by combining two approaches.
The first uses a Twitter profile archiver that is one of the components of the [Hassreden-Tracker](https://github.com/travisbrown/hassreden-tracker) project,
which was supported by [Prototype Fund](https://prototypefund.de/) in 2022.
The second involves searching the Twitter API for tweets by Twitter Blue subscribers,
with queries designed to cover areas of the Twitter graph that the first approach may miss (for example non-English-language accounts).

## Format

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

Note that affiliate verification is not tracked here.

The subscription status will be one of the following:

* `B`: Subscribed to Twitter Blue
* `U`: Unsubscribed
* `S`: Permanently suspended
* `D`: Self-deactivated

