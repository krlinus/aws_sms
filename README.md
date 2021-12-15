# aws_sms
Write a layer fir aws sms API

Complete solution in Java for sending emails using SMS/Pinpoint

Aim of this project is to create a layer on top of AWS SMS API, that will:

pick up the SMS configuration from a file
send SMS
- check status of the delivery
- do necessary follow-up action such as retry
- provide a way to configure the follow-up action

Some follow-up actions

- retry using the same config
- retry using a different config
- etc


Some configuration options
- retry after how long (for example, to avoid being throttled)
- max time to be spent on a message
- failure records to go to what DB - the particulars of the DB
- In short, explore all aspects of the API and pull up all ways to explode the scenarios and bring them under configuration. This project will tend to blow up in complexity, but keep interfaces simple to use.
- 
