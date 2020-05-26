# jupyter notebook

## turn on apache server

[link](https://www.tecmint.com/install-lamp-in-centos-7/)

```
service httpd status|start|stop|restart|reload
```

## turn on the firewall

```
_ firewall-cmd --add-port=8888/tcp
_ firewall-cmd --add-port=60001/udp
```

open firewall for jupyter notebook temporarily

## jupyter notebook config

[link](https://jupyter-notebook.readthedocs.io/en/stable/public_server.html)
[link](https://techknight.eu/2016/01/03/setup-jupyter-notebook-centosrhel-7/)

## show video in jupyter notebook

[link](https://stackoverflow.com/questions/18019477/how-can-i-play-a-local-video-in-my-ipython-notebook)

```
from IPython.display import Video
Video("./5kDNA_100x-_01_5ms_middle_z1.0_.mp4")
```


