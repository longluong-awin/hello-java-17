# Simple AWS Lambda Handler written in Java 17

When activivated by the Lambda function.  It will upper case the given string and will then writes the original given parameter value and the Java version to the Log file.

## Build
`mvn clean package`

This will out put the file: `target/hello-java-17-1.0-SNAPSHOT.jar`

Create a Java 17 Lambda function and upload this JAR file, then set the `Handler` to `dev.longluong.hj17.SimpleHandler::handleRequest` in the `Runtime Settings` section.

## Test

Specify a string in the `Event Json` section of the `Test` tab of the  lambda function, and press `Test`.  

You should see the given string converted to Uppercase.  And the Log entry.
