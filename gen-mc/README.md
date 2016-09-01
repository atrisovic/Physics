SetupProject GAUSS v49r1 --use="ProdConf"
gaudirun.py prodConf_Gauss.py

SetupProject Boole v30r1
gaudirun.py prodConf_Boole.py

* Check what platforms the app supports:

lb-sdb-query listPlatforms Moore v20r4

* Change platform

LbLogin -c x86_64-slc6-gcc48-opt

SetupProject Moore v20r4 --use="AppConfig v3r200"

LbLogin -c x86_64-slc5-gcc46-opt
SetupProject Moore v14r8p1


SetupProject Brunel v43r2p11 --use="AppConfig v3r246"


cvmfsLbLogin -c x86_64-slc6-gcc48-opt