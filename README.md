1. Before make sure the following in qcom_cfg.ini 

gEnablefwlog=1
gMulticastHostFwMsgs=1


2. Where to copy  hisi-fw

athwlan.bin   #fw binary
Data.msc      #cp ./Data.msc  /firmware/image/Data.msc


3.  cnssdiag build 

#tar xzf cnssdiag_x86.tar.gz
#tar xzf uapi.tar.gz
#tar xzf target.tar.gz 
#cd cnssdiag
#make


4.  Run cnssdiag to capture the fwlog

#insmod ./wlan.ko

#sudo ./cnss_diag -f -c -d > 1.txt 2>&1

