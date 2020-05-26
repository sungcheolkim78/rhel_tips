# imagej

## install pyimagej

following [link](https://github.com/imagej/pyimagej)

```
mvn help:effective-pom
```

In scyjava, add following lines

```
93         _logger.debug('%s found in globals', JAVA_HOME_STR)
94
95     scyjava_config.add_repositories({'scijava.public': 'https://maven.scijava.org/content/groups/public'})
96     scyjava_config.add_endpoints('net.imagej:imagej:2.0.0-rc-65')
97
98     endpoints = scyjava_config.get_endpoints()
99     repositories = scyjava_config.get_repositories()
```

following [link](https://github.com/scijava/scyjava), setting scyjava is hard part.

## what is maven?


