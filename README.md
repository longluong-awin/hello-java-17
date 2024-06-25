# Simple AWS Lambda Handler written in Java 17

When activivated by the Lambda function.  It will upper case the given string and will write the original given parameter values and the Java version in the Log file.

## Build
`mvn clean package`
This will out put the file: `target/hello-java-17-1.0-SNAPSHOT.jar`
Create a Java 17 Lambda function and upload this JAR file.

## Test

Specify a string in the `Event Json` section of the `Test` tab of the  lambda function, and press `Test`.  You should the given string converted to Uppercase.  And the Log entry.
