# Problem after update with ROBOPro >=4.4.3 "Stopped" or "Angehalten" in Test Interface Window
After update with ROBOPro >=4.4.3
- TXT role "Extension" does not work (green LED does not light up)
- the interface test shows "Angehalten" or Stopped" in the window:
![interfacetest](interfacetest.PNG)
![interfacetest](interfacetest_en.PNG)
![TXT Display](TXT_Update_10_11.png)

# Solution
Repair Steps
1. If the TXT firmware version >=4.4.4, activate SSH in the settings of TXT controller `Settings -> Arrow down -> Security -> SSH Daemon` **-> ON**

2. Download and unzip the [batch files](https://github.com/fischertechnik/txt_repair/archive/master.zip)

3. Connect TXT Controller via USB

4. Open windows console, e.g. cmd.exe

5. Execute `0_new_root.bat` to show and write down the root password from TXT controller display, Hint: Enter "y" if you see "Update cached key?" Wait about 30-60 seconds!

6. Execute `1_repair_FwUpdTxt.bat` to repair IO firmware of TXT controller
