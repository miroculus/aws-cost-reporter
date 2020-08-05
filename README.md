# AWS Cost Report

This tool will collect and create Daily & Monthly AWS cost reports and put them into [Slack](https://slack.com/)

The format should be like this

```
<date> - Amazon Elastic Compute Cloud (Instance1): $<value>
<date> - Amazon Elastic Compute Cloud (Instance2): $<value>
<date> - Amazon Elastic Compute Cloud (InstanceN): $<value>
<date> - Amazon EC2 Container Registry (ECR): <value>
<date> - Amazon Simple Storage Service: $<value>
<date> - AWS Key Management Service: $<value>
<date> - AWS Data Pipeline: $<value>
```
Total Spent: `<value>`

## Before Start

This tool uses a specific file that is generated by AWS. To activate the generation, you should activate the [Detailed billing report with resources and tags](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-reports.html#other-reports)

## Recomendations

In order to fully take advantage of the potential, you should Tag your resources accordingly, otherwise you will see a lot of this

```
<date> - Amazon Elastic Compute Cloud (): $<value>
```

## Instructions

// TO FOLLOW

## Installation

// TO FOLLOW

## Neccesary envars

`SLACK_URL`: This is the Slack URL that will be used to make the post to. Format  `https://hooks.slack.com/services/<hash>/<hash>/<hash>`

`AWS_ACCOUNT_ID`: AWS account ID. This envar will be used to download the report file

`SLACK_CHANNEL`: Target channel for the notification

`COST_REPORTS_BUCKET`: The bucket in which the report will be placed by AWS
