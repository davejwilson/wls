# Updates for AspectJ Weaver

* Download the lastest Java 1.7 version of AspectJ Waever and place it in ``
* * https://repo1.maven.org/maven2/org/aspectj/aspectjweaver/1.7.2/aspectjweaver-1.7.2.jar
* Added the `JAVA_OPTIONS` environment to the docker compose file, to add the agent
```
    environment: 
      - JAVA_OPTIONS=-javaagent:/u01/aspectjweaver-1.7.2.jar
```
