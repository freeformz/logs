# Logs

## Ideas

- Detect json vs. new line
- Batching vs. Streaming

## Carriage

> A load-carrying device from which logs are suspended and which rides back and forth along the skyline on sheaves for yarding.

cli to move logs across a network to a destination

## Hooktender

>  The working foreman in charge of a yarding crew.

Orchestrates carriages

## Destinations

### Amazon Cloudwatch Logs

Single Stream

A log stream is a sequence of log events that share the same source. Each separate source of logs into CloudWatch Logs makes up a separate log stream.

A log group is a group of log streams that share the same retention, monitoring, and access control settings. You can define log groups and specify which streams to put into each group. There is no limit on the number of log streams that can belong to one log group.

### Amazon Kinesis

Probably best to put in batches?

### Amazon Redshift



### Amazon S3 objects

Timestamped objects with a prefix

### Apache Kafka

Probably best to write batches for throughput
Can feed Google Cloud Dataflow (although not sure how)

### Google Cloud Pub/Sub

https://cloud.google.com/pubsub/
Can feed Google Cloud Dataflow

### Google Cloud Datastore

https://cloud.google.com/datastore/
Can feed Google Cloud Dataflow

### Google Stackdriver Logs

Both http REST and grpc endpoints

### Heroku Logplex format

One or more batches. Can't "stream" really as content length must be known in advance.
