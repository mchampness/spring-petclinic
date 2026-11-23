# Code Intelligence Report (minimal, grep-based)

## Build System
- Maven: pom.xml (spring-boot-starter-parent 3.5.6)
- Gradle: build.gradle (org.springframework.boot 3.5.6, Gradle wrapper 8.14.3)
- Dual build system: yes

## Spring Boot Version
3.5.6

## Java Version
17

## Size Metrics
- modules: 1
- java files: 45 (main + test)
- estimated_loc: 3631

## Jackson Usage
none (no com.fasterxml.jackson imports, no custom serializers)

## Spring Security
none

## Testing Infrastructure
- @MockBean: 0, @SpyBean: 0 (already @MockitoBean)
- @WebMvcTest: 4 classes, @DataJpaTest: 1 class
- TestRestTemplate / RestTemplateBuilder in integration tests
- Testcontainers: org.testcontainers:junit-jupiter, org.testcontainers:mysql

## Observability
- spring-boot-starter-actuator (no micrometer/otel tracing deps)

## Reactive / WebFlux
none

## Native / AOT
- PetClinicRuntimeHints (RuntimeHintsRegistrar, @ImportRuntimeHints)
- native-maven-plugin, org.graalvm.buildtools.native 0.11.1

## Build Dependencies
  org.springframework.boot:spring-boot-starter-parent
  org.springframework.boot:spring-boot-starter-actuator
  org.springframework.boot:spring-boot-starter-cache
  org.springframework.boot:spring-boot-starter-data-jpa
  org.springframework.boot:spring-boot-starter-web
  org.springframework.boot:spring-boot-starter-validation
  org.springframework.boot:spring-boot-starter-thymeleaf
  org.springframework.boot:spring-boot-starter-test
  org.springframework.boot:spring-boot-devtools
  org.springframework.boot:spring-boot-testcontainers
  org.springframework.boot:spring-boot-docker-compose
  org.springframework.boot:spring-boot-maven-plugin
  com.h2database:h2
  com.mysql:mysql-connector-j
  org.postgresql:postgresql
  javax.cache:cache-api
  com.github.ben-manes.caffeine:caffeine
  org.webjars:webjars-locator-lite
  org.webjars.npm:bootstrap
  org.webjars.npm:font-awesome
  org.testcontainers:junit-jupiter
  org.testcontainers:mysql
  jakarta.xml.bind:jakarta.xml.bind-api
  org.apache.maven.plugins:maven-enforcer-plugin
  io.spring.javaformat:spring-javaformat-maven-plugin
  org.apache.maven.plugins:maven-checkstyle-plugin
  com.puppycrawl.tools:checkstyle
  io.spring.nohttp:nohttp-checkstyle
  org.graalvm.buildtools:native-maven-plugin
  org.jacoco:jacoco-maven-plugin
  io.github.git-commit-id:git-commit-id-maven-plugin
  org.cyclonedx:cyclonedx-maven-plugin
  org.apache.maven.plugins:maven-dependency-plugin
  com.gitlab.haynes:libsass-maven-plugin
  org.eclipse.m2e:lifecycle-mapping
  io.spring.gradle:dependency-management-plugin
  org.cyclonedx.bom
  io.spring.javaformat
  io.spring.nohttp
  io.spring.javaformat:spring-javaformat-checkstyle
