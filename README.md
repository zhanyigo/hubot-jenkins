# hubot-jenkins-x

hubot-jenkins-x 在官方的 hubot-jenkins基础之上，支持了搜索目录里面的任务。目录中的任务显示为：
> 目录名::任务名

hubot-jenkins-x forked from hubot-scripts/hubot-jenkins.
hubot-jenkins-x supports jobs in folder. The job name will display like this:

>```
> <folder>::<job name>
>```

# install

```bash
npm i hubot-jenkins-x
```

# Dependencies

 None

# Configuration

* HUBOT_JENKINS_URL
* HUBOT_JENKINS_AUTH

Auth should be in the `user:password` format.

# Commands

* hubot jenkins b <jobNumber>` - builds the job specified by jobNumber. List jobs to get number.
* hubot jenkins build <job>` - builds the specified Jenkins job
* hubot jenkins build <job>, <params>` - builds the specified Jenkins job with parameters as key=value&key2=value2
* hubot jenkins list <filter>` - lists Jenkins jobs
* hubot jenkins describe <job>` - Describes the specified Jenkins job
* hubot jenkins last <job>` - Details about the last build for the specified Jenkins job