# Javalin Graalvm Test Project

The following assumes GraalVM is set up and in the path.  Make sure you have the `native-image` command available.  
You can check this by running `native-image --version`.  Run `gu install native-image` if it is not available. 

1. Create a shadow jar via gradle task

2. Run the following to generate the proper native config

```shell
 java -agentlib:native-image-agent=config-output-dir=./gvm-config -jar build/libs/graalvm-app-1.0-SNAPSHOT-all.jar
 ```

3. Run native compile via gradle task