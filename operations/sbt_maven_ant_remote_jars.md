#SBT, Maven & Ant/Ivy

a) speed by using squid:

- cache the negative objects;
    
    refresh_pattern (\-javadoc|\-sources(.jar))$    0   0% 0 negative-ttl=1440
    
- only limit localhost access

    http_port localhost:8080   
    

### Fixed Problems

- 2013/9/3: ```-Dhttp.proxyHost=localhost``` is invalid, using ```-Dhttp.proxyHost=127.0.0.1``` instead in Java application on Mac OSX 10.8.  Not sure what happenend.