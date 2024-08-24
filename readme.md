Maven goal:
Execute blow command in project terminal - table will create
User@DESKTOP-ULTO8CS MINGW64 /d/Docker-Desktop_Flyway/Project/spring-jpa-flyway (master)
$ ./mvnw -Ddatabase.username=root -Ddatabase.password=root flyway:migrate

Logs:
User@DESKTOP-ULTO8CS MINGW64 /d/Docker-Desktop_Flyway/Project/spring-jpa-flyway (master)
$ ./mvnw -Ddatabase.username=root -Ddatabase.password=root flyway:migrate
Warning: JAVA_HOME environment variable is not set.
[INFO] Scanning for projects...
[INFO]
[INFO] ----------------< com.stacktips.app:spring-jpa-flyway >-----------------
[INFO] Building spring-jpa-liquibase 0.0.1-SNAPSHOT
[INFO]   from pom.xml
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- flyway:10.10.0:migrate (default-cli) @ spring-jpa-flyway ---
[INFO] Database: jdbc:mysql://localhost:3306/flyway_test (MySQL 8.0)
[INFO] Schema history table `flyway_test`.`flyway_schema_history` does not exist yet
[INFO] Successfully validated 5 migrations (execution time 00:00.058s)
[INFO] Creating Schema History table `flyway_test`.`flyway_schema_history` ...
[INFO] Current version of schema `flyway_test`: << Empty Schema >>
[INFO] Migrating schema `flyway_test` to version "1 - add movies table"
[INFO] Migrating schema `flyway_test` to version "2 - add actor table"
[INFO] Migrating schema `flyway_test` to version "3 - add movie actor relations"
[INFO] Migrating schema `flyway_test` to version "4 - insert test data"
[INFO] Migrating schema `flyway_test` with repeatable migration "create replace movies view"
[INFO] Successfully applied 5 migrations to schema `flyway_test`, now at version v4 (execution time 00:00.302s)
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  5.937 s
[INFO] Finished at: 2024-08-24T15:06:46+05:30
[INFO] ------------------------------------------------------------------------

User@DESKTOP-ULTO8CS MINGW64 /d/Docker-Desktop_Flyway/Project/spring-jpa-flyway (master)
$



# Using Flyway for Database Migration in Spring Boot

Flyway is a popular open-source tool for managing database migrations. It makes it easier to manage and version control the database schema for your application.

Flyway supports almost all popular databases including Oracle, SQL Server, DB2, MySQL, Amazon RDS, Aurora MySQL, MariaDB, PostgreSQL and more.

In this tutorial we will create a Spring Boot application to deal with MySQL8 database migration using Flyway.  This example uses Java 17, Spring Boot 3.2.4 and MySQL 8.x. For the database operation we will use Spring boot JPA.

Read full article here: 
### [Flyway for Database Migration in Spring Boot](https://stacktips.com/articles/using-flyway-for-database-migration-in-spring-boot)


### Related topics:

* [#spring-boot](https://stacktips.com/topics/spring-boot)
* [#android](https://stacktips.com/topics/android)
* [#java](https://stacktips.com/topics/java)
* [#python](https://stacktips.com/topics/python)
* [#spring](https://stacktips.com/topics/spring)
* [#design-pattern](https://stacktips.com/topics/design-pattern)
* [#git](https://stacktips.com/topics/git)
* [#maven](https://stacktips.com/topics/maven)
