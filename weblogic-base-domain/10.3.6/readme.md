# Updates for AspectJ Weaver

* Download the lastest Java 1.7 version of AspectJ Waever and placed it in the `/u01` folder of the domain docker image build
* * https://repo1.maven.org/maven2/org/aspectj/aspectjweaver/1.7.2/aspectjweaver-1.7.2.jar
* Added the `JAVA_OPTIONS` environment to the docker compose file, as the `setDomainEnv.sh` file uses and appends its own settings to this
```
    environment: 
      - JAVA_OPTIONS=-javaagent:/u01/aspectjweaver-1.7.2.jar
```
