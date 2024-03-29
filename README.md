# SNH-C6112BN / SNH-C6410BN cameras setup instructions
## Samsung / Hanwha SNH-C6112BN   
 ![Samsung / Hanwha SNH-C6112BN](SNH-C6112BN.jpg)
 
## Samsung / Hanwha SNH-C6410BN   
 ![Samsung / Hanwha SNH-C6410BN](snh-c6410bn.png)

 1. Power on the camera and wait until the led is blue or solid red.  
 2. If you have an SNH-C6410BN you could use ethernet directly and go to number 14, or press the rear wifi button until the led is green.  
 3. Connect to the DIRECT-CAM-xxxx network, where xxxx are the last 4 digit of the cam serial number on the rear label.  
 4. Enter the wifi password that is **smartcam**  
 5. Open a internet browser an insert the address http://192.168.123.1/ that is the wifi network default gateway.  
 I used Windows 10 with internet explorer.  
 ![](smartcam1.png)  
 6. Insert the default Private Key **smartcam**
 7. Press the OK button, **don't press the keyboard enter key**!
 8. When apper a dialog box say that you must change the default Private Key respond yes.  
 9. Insert the new Private Key two times:  
 ![](smartcam3.png)  
 **Write down the new Private Key because if you lose it you cannot connect to the camera. I try reset the camera with the reset pin hole but the Private Key remain my new one and don't return to smartcam!**  
 10. Re login to the camera with the new Private Key and go to Network Setting / Wireless network:  
 ![](smartcam5.png)  
 11. Power on the wirelsee network and waith serching:  
 ![](smartcam6.png)  
 12. Choose a network from the list  
 ![](smartcam7.png)  
 13. Insert the network password:  
 ![](smartcam8.png)  
 14. Apply it and then restart the camera removing the power supply.  
 15. Wait the camera connect to your wifi network, when the light in then camera is solid blue open AngryIp Scanner or another ip scanner in a device conncted to your wifi network and start a search:  
 ![](smartcam9.png)  
 16. Search for a Samsung device that has the MAC address of your camera, the MAC address is write on a label behind the camera.  
 17. Re login to your camera with the ip that you find on scanner.  
 18. If you use Internet Explorer you can install a plugin for view the images, or use the rtsp address  
 rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile1/media.smp  
 with your favourite program like VLC or Obs.


## Video resolution and formats
URL|Video|Resolution|TBR
---|-----|----------|---
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile1/media.smp|mjpeg|1920x1080|1
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile2/media.smp|h264|640x360|10
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile3/media.smp|h264|640x360|30
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile4/media.smp|h264|1280x720|15
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile5/media.smp|h264|1920x1080|30
rtsp://admin:**yournewprivatekey**@**yourcameraaddress**/profile6/media.smp|h264|640x360|30

## Audio format
pcm_mulaw, 8000 Hz, 1 channels, s16, 64 kb/s
