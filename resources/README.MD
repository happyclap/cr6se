# Resources

This section contains information and links to resources which might be useful

## General Fixing things

* [Simplify 3D guide to print quality](https://www.simplify3d.com/support/print-quality-troubleshooting/)
    * has pretty pictures about print problems and adive on what todo
* [Teaching Tech Calibration resources](https://teachingtechyt.github.io/calibration.html)
    * provides gcodes + videos on how to calabrate your 3d printer

## Know issues and fixes

* zits and oozing on curved surfaces
    * If you find the printer is becoming a little shuttering and zits/oozing on 
    curved sufaces, this could be the answer for you --> Max resolution.
    * cura settings
    ```
        Z Seam Alignment: Shortest
        Compensate Wall Overlaps: Off
        Maximum Resolution: 0.5 mm
    ```
    * [Great thread on this](https://community.ultimaker.com/topic/25388-zits-on-curved-surfaces-crazy-toolpath/)
    * [CNC Kitchen youtube video on this](https://youtu.be/Hvw3DrVAeTA)
* Heating Failed Error
    * This is where a "Heating Error" message is displayed on the touchscreen. 
    * Two possible fixes:
        * [PID autotune](https://teachingtechyt.github.io/calibration.html#pid) - this
        runs the automated configuration on the heating of the nozzel and bed
        ```
        M303 E0 S220 C5 U1
        ```
        * Upgrade your firmware, refer below (this fixed my issues)
* Changing nozzle and tube
    * Dont forget to heat the nozzle ;)
    * [Creality video tutorial](https://youtu.be/XGKRg7Q1mPE)
    

## Upgrading Firmware

Downloading firmware:
* [Creality Offical](https://www.creality.com/download) - find CR6se and download
* [Community Firmware]() - community version of firmware.

General process for firmware:
* down firmware
* copy .bin file to an empty SD card. at time of writing, file was:
    ```
    CR-6SE-V1.0.3.6.bin
  ```
* turn machine off, insert SD card, turn machine on. it will take some time to load
the new firmware
* your done. 

Videos:
* [updating screen firmware youtube](https://youtu.be/RGDNItCmJpw)
* [updating machine firmware youtube](https://youtu.be/BXqSxsVwfCg)
