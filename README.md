<!---
Current Directory : /in28Minutes/git/spring-boot-examples/spring-boot-web-application-bootstrap-jquery
-->

## Helping You Master Cloud, Full Stack and Microservices 

> **30** Courses, **5** Learning Paths & **350K** Learners 

You do not learn to drive by watching Tom Cruise drive at 300 kmph! You have to **get your hands dirty**.

At in28minutes, **Our goal** is to help you learn and re-skill Spring Boot, Microservices, Full Stack, Cloud (AWS), Docker and Kubernetes with **hands-on, practical courses**.

We have build solutions to help you master Cloud, Full Stack and Microservices in **1-3 Months**.

You can check out all our courses here - [https://github.com/in28minutes/learn](https://github.com/in28minutes/learn)

## Learn from the Top 5 Best Selling Courses

- [Master DevOps with Docker, Kubernetes and Azure DevOps](https://links.in28minutes.com/DevOps-SBT)
- [Kubernetes for Java Developers on Google Cloud](https://links.in28minutes.com/SBT-Footer-Kubernetes)
- [Docker for Java Developers - with Spring Boot Microservices](https://links.in28minutes.com/SBT-Footer-Docker)
- [Learn AWS - Deploy Java Spring Boot to AWS Elastic Beanstalk](https://links.in28minutes.com/SBT-Footer-AWS-BeanStalk)
- [Master Microservices with Spring Boot and Spring Cloud](https://links.in28minutes.com/SBT-Footer-Microservices)
- [Learn Java Full Stack with Spring Boot and React](https://links.in28minutes.com/SBT-Footer-React)


## Reskill with the Amazing in28Minutes Learning Paths

- [Learning Path 01 - Spring and Spring Boot Web Applications and API Developer](https://links.in28minutes.com/in28minutes-LP-01)
- [Learning Path 02 - Full Stack Developer with Spring Boot, React & Angular](https://links.in28minutes.com/in28minutes-LP-02)
- [Learning Path 03 - Cloud Microservices Developer with Docker and Kubernetes](https://links.in28minutes.com/in28minutes-LP-03)
- [Learning Path 04 - Learn Cloud with Spring Boot, AWS, Azure and PCF](https://links.in28minutes.com/in28minutes-LP-04)
- [Learning Path 05 - Learn AWS with Microservices, Docker and Kubernetes](https://links.in28minutes.com/in28minutes-LP-05)



### More Courses and Videos From in28Minutes
- https://github.com/in28minutes/learn

## Complete Code Example


### /pom.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>

	<groupId>com.in28minutes.springboot.web.application</groupId>
	<artifactId>spring-boot-web-application-bootstrap-jquery</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<packaging>jar</packaging>

	<name>spring-boot-web-application-bootstrap-jquery</name>
	<description>Spring Boot Tutorial - Adding Bootstrap and JQuery to Web Application</description>

	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.0.0.RELEASE</version>
		<relativePath /> <!-- lookup parent from repository -->
	</parent>

	<properties>
		<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
		<project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>
		<java.version>1.8</java.version>
	</properties>

	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<dependency>
			<groupId>org.webjars</groupId>
			<artifactId>bootstrap</artifactId>
			<version>3.3.6</version>
		</dependency>

		<dependency>
			<groupId>org.webjars</groupId>
			<artifactId>bootstrap-datepicker</artifactId>
			<version>1.0.1</version>
		</dependency>

		<dependency>
			<groupId>org.webjars</groupId>
			<artifactId>jquery</artifactId>
			<version>1.9.1</version>
		</dependency>

		<dependency>
			<groupId>org.apache.tomcat.embed</groupId>
			<artifactId>tomcat-embed-jasper</artifactId>
			<scope>provided</scope>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
			<scope>runtime</scope>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>

	<repositories>
		<repository>
			<id>spring-snapshots</id>
			<name>Spring Snapshots</name>
			<url>https://repo.spring.io/snapshot</url>
			<snapshots>
				<enabled>true</enabled>
			</snapshots>
		</repository>
		<repository>
			<id>spring-milestones</id>
			<name>Spring Milestones</name>
			<url>https://repo.spring.io/milestone</url>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
		</repository>
	</repositories>

	<pluginRepositories>
		<pluginRepository>
			<id>spring-snapshots</id>
			<name>Spring Snapshots</name>
			<url>https://repo.spring.io/snapshot</url>
			<snapshots>
				<enabled>true</enabled>
			</snapshots>
		</pluginRepository>
		<pluginRepository>
			<id>spring-milestones</id>
			<name>Spring Milestones</name>
			<url>https://repo.spring.io/milestone</url>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
		</pluginRepository>
	</pluginRepositories>


</project>
```
---

### /src/main/java/com/in28minutes/springboot/tutorial/basics/application/configuration/SpringBootWebApplicationBootstrapJqueryApplication.java

```java
package com.in28minutes.springboot.tutorial.basics.application.configuration;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class SpringBootWebApplicationBootstrapJqueryApplication {

	public static void main(String[] args) {
		SpringApplication.run(SpringBootWebApplicationBootstrapJqueryApplication.class, args);
	}
}
```
---

### /src/main/java/com/in28minutes/springboot/tutorial/basics/application/configuration/WelcomeController.java

```java
package com.in28minutes.springboot.tutorial.basics.application.configuration;
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class WelcomeController {	
	@RequestMapping("/welcome")
	public String loginMessage(){
		return "welcome";
	}
}
```
---

### /src/main/resources/application.properties

```properties
spring.mvc.view.prefix=/WEB-INF/jsp/
spring.mvc.view.suffix=.jsp
logging.level.org.springframework.web=INFO
```
---

### /src/main/resources/static/css/custom.css

```css
body {
    background-color: lightblue;
}
```
---

### /src/main/resources/static/js/custom.js

```js
alert("I'm active");
```
---

### /src/main/webapp/WEB-INF/jsp/welcome.jsp

```
<html>
<head>
	<title>Welcome</title>
	<link href="webjars/bootstrap/3.3.6/css/bootstrap.min.css"
		rel="stylesheet">
	<link href="css/custom.css"
		rel="stylesheet">
</head>
<body>
	<div class="container">
		<table class="table table-striped">
			<caption>Your todos are</caption>
			<thead>
				<tr>
					<th>Description</th>
					<th>Target Date</th>
					<th>Is it Done?</th>
					<th>Edit</th>
					<th>Delete</th>
				</tr>
			</thead>
			<tbody>
					<tr>
						<td>Todo 1</td>
						<td>10/12/2017</td>
						<td>No</td>
						<td><a class="btn btn-warning" href="/edit-todo">Edit Todo</a></td>
						<td><a class="btn btn-warning" href="/delete-todo">Delete Todo</a></td>
					</tr>
			</tbody>
		</table>
		<div>
			<a class="btn btn-default" href="/add-todo">Add a Todo</a>
			
		</div>
		<script src="webjars/jquery/1.9.1/jquery.min.js"></script>
		<script src="webjars/bootstrap/3.3.6/js/bootstrap.min.js"></script>
		<script src="js/custom.js"></script>
	</div>
</body>
</html>
```
---

### /src/test/java/com/in28minutes/springboot/tutorial/basics/application/configuration/SpringBootWebApplicationBootstrapJqueryApplicationTests.java

```java
package com.in28minutes.springboot.tutorial.basics.application.configuration;

import org.junit.Test;
import org.junit.runner.RunWith;
import org.springframework.boot.test.context.SpringBootTest;
import org.springframework.test.context.junit4.SpringRunner;

@RunWith(SpringRunner.class)
@SpringBootTest
public class SpringBootWebApplicationBootstrapJqueryApplicationTests {

	@Test
	public void contextLoads() {
	}

}
```
---
