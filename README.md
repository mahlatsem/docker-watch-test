# docker-watch-test

To test run `mvn` which will execute the defaultGoal `clean package docker:build docker:start docker:watch`

Whenever you run `mvn package`, the container should be restarted and all the configuration that runs for start 
should also run for the restarted container, i.e. `<wait>` configuration, but this doesn't happen in io.fabric8:docker-maven-plugin:0.26.1
