# Maltese (Malware Traffic Emulating Software)
Maltese is a tool that is used to emulate malicious traffic generated by a given malware.
>Developed using Python 3.4.3

##Maltese Command line options
####Root commands
```
usage: maltese.py [-h] {dga,replay} ...

optional arguments:
  -h, --help    show this help message and exit

commands:
  {dga,replay}
    dga         Execute DGA plugins
    replay      Execute Replay plugins
```

####DGA options
```
usage: maltese.py dga [-h] -p {necurs,sampledga} [-l {error,warning,info,debug}]

optional arguments:
  -h, --help                        show this help message and exit
  -l {error,warning,info,debug}     Logging level. Default is error

required arguments:
  -p {necurs,sampledga}             DGA Plugin module to run
```

####Replay options
```
usage: maltese.py replay [-h] -p {list,pcap} -i INPUT
                      [-l {error,warning,info,debug}]

optional arguments:
  -h, --help            show this help message and exit
  -l {error,warning,info,debug}
                        Logging level. Default is error

required arguments:
  -p {list,pcap}        Replay Plugin module to run
  -i INPUT              Input file for replay.
```