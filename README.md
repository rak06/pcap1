# monitor capture buffer <name1> size 12400                   ---->creating buffer
monitor capture point ip cef <name2> port-channel 1.102 both --->selecting interface
monitor capture point associate <name2> <name1> 
monitor capture point start all
monitor capture point stop all
sh monitor capture buffer all parameters

monitor capture buffer <name1> export tftp://ip address/test.pcap --> moving to tftp

no monitor capture buffer <name1>  ---> delete the buffer after testing
no monitor capture point ip cef <name2> port-channel 1.102 both 
