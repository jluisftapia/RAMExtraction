# RAM Extraction Tool
This Repository contains the Instructions and tools to create a USB scraper tool used for dumping the contents from RAM memory module from a computer.


### - Get a USB with enough capacity to store the memory from the target PC, this can work on a wide variety of DDR2 or DDR3 RAM modules

For example, if the target Machine has the following characteristic: 

Type of RAM:  DDR2
Capacity: 1GB

We should use a USB drive with 2 GB of capacity.

### - Download the contents of this repository 

### - Contents explanation:

> a) pre-compiled 32-bit version of the scraper.bin
Notice: This scraper works only for file systems of 32 bit and will only save a maximum of 4GB of memory, also important to notice use a USB 3.0 drive with a fast write speed is a good idea since slower type can take longer time.

> b) RMPrepUSB_Portable_v2.1.741a.zip. Unzip this file and which contains several tools from those select "RMPREPUSB.exe" this writes to the USB drive on the sector 0 which will make our device the boot drive.

## Building the USB

### - On a windows PC we run the program RMPrepUSB

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/RMPrepUSB.png)

1) Make sure first that your USB appears at the top of the window
2) Select the from Image Tools the option File-> Drive 
3) Search the scraper.bin file and click Open
4) Click OK on the following windows until completed the File to Drive process.

As observed in the following image:
![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/USB-preparation.png)

### - Once finished the USB writing process, take the computer on sleeping mode, insert the USB then shut it down by removing the battery

#### Optionally  With the RAM module exposed you can freeze it with the help of a can of compressed air, discharging the content with the Air Can on inverted (Upside Down) position resulting in the spraying of liquid on to the surface. 

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/compresedair.png)

This way you can freeze the RAM memory as much as possible:

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/freezemem.png)

Warning: The liquid, when released from the can on this position, boils at a very low temperature, rapidly cooling any surface it touches, this can be harmful if is directly released against the human body.   

### - Then power on the PC by plug it into the AC adapter, pressing F12 or consult first the corresponding function key for the specific computer model to access into the booting menu

Here is a list of possible hotkeys depending on the brand and model.

https://www.disk-image.com/faq-bootmenu.htm

### - Start from the external device and see how it starts dumping the RAM memory... It may take a long time depending on the memory from the target.

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/dumprocess.jpg)

You can find next to the link with the video from the experiment performed by us: 

https://youtu.be/FG8QXaqwBcQ

### - The process of recovery the content of the USB is described next

> 1. Remove the USB right after finishes the dump process this is because the process can start again and this would delete the contents already dumped.
> 2. To see the contents of the RAM was used first PhotoRec 7.1 Data Recovery Utility for Windows.

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/photorec.png)

> 3. Then the recovered files are refined with File Recovery for Windows

![](https://github.com/jluisftapia/RAMExtraction/blob/master/Images/FileRecovery.png)

### -Additionally it is possible to dump the RAM contents into a ".img" file using DD, with that image file we can use it later or store it as evidence.
