# Natural Language Processing with Disaster Tweets


## Overview

Classification of Tweets if they report disaster or not. This we can find if there is disaster occuring currently and report location along with sending help. 

## Motivation

Twitter seems to first place people report on any public level events. Finding tweets that have reported disaster on real time will help us to send help at given location.

## Success Metrics 

Imporved response time of Police and other public services.


## Requirements & Constraints

Tweets could ambigious or misinformation on location resulting in panic, A tweet which meets more than 0.7 only then we can classify as disaster tweet. Update based on customer demand. 

Since it will applied on Real Time data, we need model to have fast response time. Low Latency. Also expecting a batch of tweets to processed together. Allowing upto 32 tweets to be processed at one time. Larger the model more the sample size.


## Methodology


### Problem Statement

A simple supervised classification problem for real time data stream.


### Data

Data is downloaded from kaggle, we will be performing EDA over it to find patterns on which model to apply and how to solve it.

Input Data will be a raw tweet with locatiion if available. Raw tweet will contian hashtags, special symbols.

### Techniques 

Will be starting with Simple Logistic Regression and build end to end pipeline.

### Experimentation & Validation.


### Human-in-loop

We could have a poll question if the tweet is true. So it gets publicly acknowledged. 


## Implementation

![High Level Design](./docs/Screenshot%202022-09-12%20at%2014-10-15%20Blank%20diagram%20Lucidchart.png)


### Infra

DB - Postgres
Docker
AWS Lambda
TBD

### Performance (Throughput, Latency)
TBD

### Security

TBD

### Data Privacy

Social media post, no consent taken.

### Monitoring & Alarms.

If the number of predictions done by model are totally opposite of twitter poll on same tweet. We set alarm to update the model or signify.

## Integration Points

TBD

### Risks & Uncertainties

TBD

## Appendix

TBD

