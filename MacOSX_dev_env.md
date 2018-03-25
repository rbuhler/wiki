# Development Environment
## System Variables

### JAVA Development Kit
#### Steps
- Download 8 
  - [jdk 8.162](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html?printOnly=1)
- Install;
- Update $JAVA_HOME;
  - vi ~/.bash_profile
```
# JAVA
JAVA_HOME=`/usr/libexec/java_home -v 1.8.0_162`
export PATH=$JAVA_HOME/bin:$PATH 
```
