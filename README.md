# Graalvm Test Project

The following assumes GraalVM is setup and in the path.

1. Create a shadow jar via gradle task

2. Run the following to generate the proper native config

```shell
 java -agentlib:native-image-agent=config-output-dir=./gvm-config -jar build/libs/graalvm-app-1.0-SNAPSHOT-all.jar
 ```

3. Run native compile via gradle task