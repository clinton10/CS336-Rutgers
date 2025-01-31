# CS336 Sample Project - Gradle

This is a port of the CS336 sample project that uses Gradle to create the output `.war` file.

## Prerequites

-  Java 8+
-  [Gradle](https://gradle.org/)
-  [Apache Tomcat](http://tomcat.apache.org/)
-  MySQL Workbench
-  MySQL Server

## Instructions

1. Download and navigate into the project.
2. Execute the SQL file in the `Resources` directory as the instructions states in MySQL Workbench.
3. Change the JDBC Connection String, database username and database password in [`ApplictionDB.java`](src/main/java/com/cs336/pkg/ApplicationDB.java).
4. To generate the `.war` file, run

   ```sh
   gradle clean build
   ```

   If one doesn't have Gradle installed, run

   ```sh
   ./gradlew clean build
   ```

   in Bash or

   ```sh
   .\gradlew.bat clean build
   ```

   in Powershell.

5. The `.war` file would be in the newly created `build/libs` directory.
