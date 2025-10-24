

# update the pom.xml file acc to your database
<!-- Databases -->
        <!-- <dependency>
            <groupId>org.postgresql</groupId>
            <artifactId>postgresql</artifactId>
            <scope>runtime</scope>
        </dependency>
    
        <dependency>
            <groupId>com.mysql</groupId>
            <artifactId>mysql-connector-j</artifactId>
            <scope>runtime</scope>
        </dependency>
    
        <dependency>
            <groupId>com.h2database</groupId>
            <artifactId>h2</artifactId>
            <scope>runtime</scope>
        </dependency> -->


# update the application.properties file
spring.application.name=sutherland-lms-app

server.port : 8484
server.servlet.contextPath : /lms

#database configuration

---- ORACLE ----
spring.datasource.url=jdbc:oracle:thin:@10.33.61.109:1521:xe
spring.datasource.username=test
spring.datasource.password=test123
spring.datasource.driver-class-name=oracle.jdbc.driver.OracleDriver
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.Oracle10gDialect

<!-- 
# ---- MYSQL ----
# spring.datasource.url=jdbc:mysql://localhost:3306/mysqldb
# spring.datasource.username=root
# spring.datasource.password=root
# spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
# spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect

# ---- POSTGRESQL ----
# spring.datasource.url=jdbc:postgresql://localhost:5432/postgresdb
# spring.datasource.username=postgres
# spring.datasource.password=postgres
# spring.datasource.driver-class-name=org.postgresql.Driver
# spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

# ---- H2 (In-Memory) ----
# spring.datasource.url=jdbc:h2:mem:testdb
# spring.datasource.driver-class-name=org.h2.Driver
# spring.datasource.username=sa
# spring.datasource.password=
# spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.H2Dialect


spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true -->
