'bl702_cklink_whole_img_v2.2.bin':

- Turn sipeed rv debugger plus to CK-Link Lite debugger.
- Program by:
  + `bflb-mcu-tool --chipname=bl702 --interface=uart --port=/dev/ttyACM0 --baudrate=2000000 --firmware=bl702_cklink_whole_img_v2.2.bin`
  Or
  + `blisp iot -c bl70x --reset -s bl702_cklink_whole_img_v2.2.bin -l 0x0`
- It is from https://github.com/bouffalolab/bl_mcu_sdk/tree/master/tools/cklink_firmware. 
- only binary release.


'usb2uartjtag_bl702.bin' and 'usb2dualuart_bl702.bin':

- Turn sipeed rv debugger plus to jtag+uart or dual uart.
- Program firmware by:
  + `bflb-mcu-tool --chipname=bl702 --interface=uart --port=/dev/ttyACM0 --baudrate=2000000 --firmware=usb2uartjtag_bl702.bin`
- It is built from https://github.com/sipeed/RV-Debugger-BL702/tree/main/firmware

'ft2232d.cfg':
- OpenOCD cfg file for usb2uartjtag firmware.

'ft2232h.cfg':
- OpenOCD cfg file for usb2dualuart firmware.
