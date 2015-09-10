#NOTE: Under linux make sure you use *sudo* to access any ftdi devices.
```
sudo ./fpgaprog -jv
```
##To compile (ubuntu): 
```
    sudo apt-get install libftdi-dev
    cd src
    make
```
##To run:
```
Usage:./fpgaprog [-v] [-j] [-f <bitfile>] [-b <bitfile>] [-s e|v|p|a] [-c] [-C] [-r] [-A <addr>:<binfile>]
   -h                   print this help
   -v                   verbose output
   -j                   Detect JTAG chain, nothing else
   -d                   FTDI device name
   -f <bitfile>         Main bit file
   -b <bitfile>         bscan_spi bit file (enables spi access via JTAG)
   -s [e|v|p|a]         SPI Flash options: e=Erase Only, v=Verify Only,
                        p=Program Only or a=ALL (Default)
   -c                   Display current status of FPGA
   -C                   Display STAT Register of FPGA
   -r                   Trigger a reconfiguration of FPGA
   -a <addr>:<binfile>  Append binary file at addr (in hex)
   -A <addr>:<binfile>  Append binary file at addr, bit reversed
```
