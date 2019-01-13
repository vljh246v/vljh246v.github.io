---
layout: post
title: Spring boot 톰캣 -> jetty
subtitle: 톰캣 -> jetty
tags: [post, jetty, eclipse, 공부, 웹컨테이너, spring boot, spring]
comments: true
image: /img/jetty.png
---



`spring-boot-starter-web`을 사용하면 자동으로 embedded Tomcat이 아티팩트에 추가된다.  
Tomcat을 기본 웹 컨테이너로 사용하지만 만약 Tomcat 말고 Jetty로 컨테이너를 변경하고 싶다면  
아래와 같이 pom.xml에 내용을 변경해 주면 된다.  
(maven 을 기준으로 작성)
  
___
  
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-web</artifactId>
	<exclusions>
		<exclusion>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-tomcat</artifactId>
		</exclusion>
	</exclusions>
</dependency>
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-jetty</artifactId>
</dependency>
```

