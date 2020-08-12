# STM32L152C-DISCO
How to get startet with the STM32L132C-DISCO board by STMicroelectronics.

For programming the STM32L152C-DISCO board, an IDE (Integrated Development Environment) 
is required.
# Download the IDE
STMicroelectronic recommendes the **System Workbench for STM32**.
The following link is to my shared onedrive-folder, where the download for the **SW4STM32 System Workbench for STM32** Windows-Version is.

https://1drv.ms/f/s!Aoh3weszM5s2aphTEA8xX2PuYeA

The official link to the download via the ST-Website is:
https://www.st.com/en/development-tools/sw4stm32.html#get-software

After clicking on the link at the ST-Website, you get to the OpenSTM32 Community.
After creating an account and logging in, you click on **System Workbench for STM32** at the menu on the left side.
Now you can choose your download for your OS.
#IDE
There is the **STM32CubeIDE** by ST and the **System Workbench dor STM32**. Both of them are Eclipsed based, but the System Workbench dor STM32 is easier to use with the STM32L152C-DISCO, becuase you can chose exact the STM32L152C-DISCO. The 

# Step-by-Step instruction for the STM32CubeIDE
(Follow the steps to get started as quick as possible, if you want to know more about the steps, read the description below the particular step.)

STM32CubeMX
  1.  Download and install the **STM32CubeMX** software.
  
  2.  Click under **Start My project from STBoard** on the **ACCESS TO BOARD SELECTOR**.
  3.  Click on the field next to the magnifying glass and type: **32L152CDISCOVERY**.
  4.  Click on the board and click on **Start Project**.
  5.  A pop-up-window comes up and askes for: **Initialize all peripherals with their default Mode ?**, click **Yes**.
    Now you are in the  **Pinout & Configuration** tab, where you can change the the pinout and configurations, BUT THIS IS A DEMOBOARD, SO THE PINOUT AND THE      CONFIGURATION IS ALREADY PRESET FOR THE **STM32L152C-DISCO**, SO IT IS NOT RECOMMENDED TO CHANGE THEM!
  
  6.  The **Clock Configuration** tab is also already preset for you in this particular case, so you do not have to change anything here.
  7.  In the **Project Manager** tab you can set a name for your project, a location, where your project is stored. For beginning chose **Basic** at the **Application Structure**, and make sure, the checkbox **Do not generate the main()** is NOT checked.
  8.  The next step is to set your toolchain/IDE. In my chase it is **STM32CubeIDE** because I am using the STM32CubeIDE. Maybe you have to change the **Firmware Location** such as in my chase.
  9.  Under the **Tools** tab is a power consumtion calculator, but there is nothing to change.
  10. Click on **GENERATE CODE** above the **Tools** tab.
  11. A popup window appears, when the code is successfully generated.

STM32CubeIDE
  12. Click on **File**.
  13. Click on **New**.
  14. Click on **STM32 Project from an Existing STM32CubeMX Configuration File (.ioc)**.
  15. Under **STM32CubeMX .ico file** click on **Browse** and chose your folder, where you have saved your project that we created earlier with the 32CubeMX software. The project name should be loaded automatically.
  16. Under **Options** I am chosed **C** as my targeted language, but chose your language you are familiar with.
  17. Click on **Finish**. In my chase the firmware was not compatible, so I clicked "Continue and the firmware downloaded automatically.

# GPIO TEST (Article is in Beta Phase)

Click on your project, click on "Core", click on **SRC** and doubleclick pon **main.c**.

An exact discription is **Project/Drivers/SRC/stm32l1xx_hal_gpio.c**
