# [Cloudwatch] Logs

List streams:

```bash
aws logs describe-log-streams --log-group-name '/aws/elasticbeanstalk/example/var/log/nodejs/nodejs.log' | jq -r '.logStreams[] .logStreamName'
```

Get latest log messages:

```bash
aws logs get-log-events --log-group-name '/aws/elasticbeanstalk/example/var/log/nodejs/nodejs.log' --log-stream-name 'i-123456789' | jq -r '.events[] .message'
```