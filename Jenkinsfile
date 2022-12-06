#!/usr/bin/env groovy

dockerfile {
    dockerPush = true
    dockerRepos = ['confluentinc/cp-kafka-mqtt',]
    mvnPhase = 'package'
    mvnSkipDeploy = true
    nodeLabel = 'docker-debian-jdk8-compose'
    slackChannel = 'connect-notification'
    upstreamProjects = []
    dockerPullDeps = ['confluentinc/cp-base-new']
    usePackages = true
    cron = '' // Disable the cron because this job requires parameters
    cpImages = true
    osTypes = ['ubi8']
    disableConcurrentBuilds = true
}
