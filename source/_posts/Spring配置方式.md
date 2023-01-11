---
title: Spring配置方式
categories: [Spring]
description: Spring的配置发展
date: 2022-12-23
tags:
  - 学习
  - Java
  - Spring
---
## Spring的配置发展
  Spring IOC有一个非常核心的概念——**Bean**。由Spring容器来负责对Bean的实例化，装配和管理。XML是用来描述Bean最为流行的配置方式。
  但随着Spring的日益发展，越来越多的人对Spring提出了批评。“Spring项目大量的烂用Xml”就是最为严励的一个批评。由于Spring会把几乎所有的业务类都以Bean的形式配置在XML文件中，因此产生了大量的XML文件，使得整个项目变得更加复杂，并且使Bean失去了**编译时的类型安全检查**。 
  随着JDK1.5的发布，其中引入了一个非常重要的特性——**Annotations**(注解)。注释是源代码的标签，这些标签可以在源代码层进行处理或通过编译器把它熔入到class文件中。在JDK1.5以后的版本中，注释成为了一个主要的配置选项。Spring使用注释来描述Bean的配置与采用XML相比，因类注释是在一个类源代码中，可以获得类型安全检查的好处。可以良好的支持重构。
### 第一阶段 Xml文件
  Spring1.x时代，开发基本上都是使用Xml文件配置Bean。但是随着项目不断的增大，产生了大量的配置文件，需要频繁的在类和配置文件进行切换，给开发人员带来了不必要的成本。

### 第二阶段 注解配置

  Spring2.x时代，随着Jdk1.5带来了对注解的支持，Spring也随之提供了声明Bean的注解, 大大的减少了配置文件，同时也大大简化了项目的开发。
那么，问题来了，究竟是应该使用xml还是注解呢？
> 1. 应用的基本配置用xml，比如：数据源、资源文件等
> 2. 业务开发用注解，比如：Service中注入bean等IOC
> 3. AOP（切面编程）建议用XML
### 第三阶段 Java配置
  Spring3.x时代到现在，Spring提供了Java配置的能力，使Java配置更好的理解，现在都推荐使用Java配置。

## Java配置

### 相关注解

>  @Configuration、@ConditionalOnProperty、@ConditionalOnClass、@ConfigurationProperties、@PropertySource、@Value、@Profile、@EnableConfigurationProperties、@EnableAutoConfiguration、@SpringBootConfiguration、@SpringBootApplication
