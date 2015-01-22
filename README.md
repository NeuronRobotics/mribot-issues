# mribot-issues
### program card

If you loose power and need to re-program card.
attatch JTAG cable to card and do this.
if you have problems then reboot and email me.

CD to `~/git/thoughtstabber/FPGASources`
run `./progcard.sh`

you should see something like this
```
aimlab@mri-controller:~/git/thoughtstabber/FPGASources$ ./progcard.sh 
. /opt/Xilinx/14.6/ISE_DS/common/.settings64.sh /opt/Xilinx/14.6/ISE_DS/common
. /opt/Xilinx/14.6/ISE_DS/EDK/.settings64.sh /opt/Xilinx/14.6/ISE_DS/EDK
. /opt/Xilinx/14.6/ISE_DS/PlanAhead/.settings64.sh /opt/Xilinx/14.6/ISE_DS/PlanAhead
. /opt/Xilinx/14.6/ISE_DS/ISE/.settings64.sh /opt/Xilinx/14.6/ISE_DS/ISE
Release 14.6 - iMPACT P.68d (lin64)
Copyright (c) 1995-2013 Xilinx, Inc.  All rights reserved.
Preference Table
Name                 Setting             
StartupClock         Auto_Correction     
AutoSignature        False               
KeepSVF              False               
ConcurrentMode       False               
UseHighz             False               
ConfigOnFailure      Stop                
UserLevel            Novice              
MessageLevel         Detailed            
svfUseTime           false               
SpiByteSwap          Auto_Correction     
AutoInfer            false               
SvfPlayDisplayComments false               
INFO:iMPACT - Digilent Plugin: Plugin Version: 2.4.4
INFO:iMPACT - Digilent Plugin: no JTAG device was found.
AutoDetecting cable. Please wait.
*** WARNING ***: When port is set to auto detect mode, cable speed is set to
default 6 MHz regardless of explicit arguments supplied for setting the baud
rates
Connecting to cable (Usb Port - USB21).
Checking cable driver.
File version of /opt/Xilinx/14.6/ISE_DS/ISE/bin/lin64/xusbdfwu.hex = 1030.
File version of /etc/hotplug/usb/xusbdfwu.fw/xusbdfwu.hex = 1030.
 Using libusb.
 Kernel release = 3.13.0-24-lowlatency.
 Max current requested during enumeration is 300 mA.
Type = 0x0005.
 Cable Type = 3, Revision = 0.
 Setting cable speed to 6 MHz.
Cable connection established.
Firmware version = 2401.
File version of /opt/Xilinx/14.6/ISE_DS/ISE/data/xusb_xp2.hex = 2401.
Firmware hex file version = 2401.
PLD file version = 200Dh.
 PLD version = 200Dh.
Type = 0x0005.
ESN option: 000016E5F14801.
Identifying chain contents...'0': : Manufacturer's ID = Xilinx xcf04s, Version : 13
INFO:iMPACT:1777 - 
   Reading /opt/Xilinx/14.6/ISE_DS/ISE/xcf/data/xcf04s.bsd...
INFO:iMPACT:501 - '1': Added Device xcf04s successfully.
----------------------------------------------------------------------
----------------------------------------------------------------------
'1': : Manufacturer's ID = Xilinx xc6slx9, Version : 2
INFO:iMPACT:1777 - 
   Reading /opt/Xilinx/14.6/ISE_DS/ISE/spartan6/data/xc6slx9.bsd...
INFO:iMPACT:501 - '1': Added Device xc6slx9 successfully.
----------------------------------------------------------------------
----------------------------------------------------------------------
done.
Elapsed time =      0 sec.
Elapsed time =      0 sec.
'1': Loading file 'board-test/top.bit' ...
done.
INFO:iMPACT:2257 - Startup Clock has been changed to 'JtagClk' in the bitstream
   stored in memory,
   but the original bitstream file remains unchanged.
UserID read from the bitstream file = 0xFFFFFFFF.
Data width read from the bitstream file = 1.
----------------------------------------------------------------------
INFO:iMPACT:501 - '1': Added Device xc6slx9 successfully.
----------------------------------------------------------------------
----------------------------------------------------------------------
Maximum TCK operating frequency for this device chain: 15000000.
Validating chain...
Boundary-scan chain validated successfully.
'1': Programming device...
 LCK_cycle = NoWait.
LCK cycle: NoWait
done.
'1': Reading status register contents...
[0] CRC ERROR                                                              :    
    0
[1] IDCODE ERROR                                                           :    
    0
[2] DCM LOCK STATUS                                                        :    
    1
[3] GTS_CFG_B STATUS                                                       :    
    1
[4] GWE STATUS                                                             :    
    1
[5] GHIGH STATUS                                                           :    
    1
[6] DECRYPTION ERROR                                                       :    
    0
[7] DECRYPTOR ENABLE                                                       :    
    0
[8] HSWAPEN PIN                                                            :    
    1
[9] MODE PIN M[0]                                                          :    
    1
[10] MODE PIN M[1]                                                         :    
    1
[11] RESERVED                                                              :    
    0
[12] INIT_B PIN                                                            :    
    1
[13] DONE PIN                                                              :    
    1
[14] SUSPEND STATUS                                                        :    
    0
[15] FALLBACK STATUS                                                       :    
    0
INFO:iMPACT:2219 - Status register values:
INFO:iMPACT - 0011 1100 1110 1100 
'1': Verifying  device...INFO:iMPACT:2495 - Readback Size is 2722512.
done.
'1': Verification completed successfully.
 LCK_cycle = NoWait.
LCK cycle: NoWait
INFO:iMPACT:579 - '1': Completed downloading bit file to device.
INFO:iMPACT:188 - '1': Programming completed successfully.
 LCK_cycle = NoWait.
LCK cycle: NoWait
INFO:iMPACT - '1': Checking done pin....done.
'1': Programmed successfully.
Elapsed time =      3 sec.
----------------------------------------------------------------------
----------------------------------------------------------------------

```
