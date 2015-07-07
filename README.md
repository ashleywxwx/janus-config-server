# Project Janus

## Config Server

### Built on Spring Boot Cloud Config

#### Load properties from git

To load properties from git, use the standard spring-boot:run

    mvn spring-boot:run
    
#### Load properties from file

To load properties from the file system, set the active profile to native

    mvn spring-boot:run -Dspring.profiles.active=native

This forces the config server to search the file system at the location specified with the property 

    spring.cloud.config.server.native.searchLocations
