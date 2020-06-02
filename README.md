# Test_PHP

This project covers 3 Testcases.
-PHP Travels user registration
-Login and Logout
-Verify details page

We can trigger the test cases from TestRunner file. Go to this file. File location is: src/test/java/testRunner/TestRunner.java
To trigger:
Right click, select Run As -> TestNG Test

To run in different env:
-Go to end of the pom.file
-Set the value for activeByDefault key as true in the corresponding env profile
-Example, For SIT env:

<profile>
  <activation>
    <activeByDefault>true</activeByDefault>
  </activation>
  <id>sit</id>
  <properties>
    <env>sit</env>
  </properties>
</profile>

Note: Build the project after updating this in pom file.

To run in different browser:
-Set the value for browser key as chrome or firefox in the config.properties file
-Example,
browser=chrome
(or)
browser=firefox
-File location is: src/main/resources/config.properties
