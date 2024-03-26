# MB Smart Android Insallation Troubleshooting:

## Known installer error codes:

- A screen that looks like either one of these:
  ![DPM error of reinstalling while removal is in process](./img/BeingRemoved2.png)
  ![Regular error of owner being installed while removal is in progress](./img/ReinstallRemovalInProgress.png)
  Indicates that you are trying to install the filter while the device owner that was present is currently being removed, and waiting a minute or two would be recommended.

- This installer error:
  ![UnknownAdmin error](./img/UnkwownAdmin.png)
  Indicates that the device admin was not recognized, which could be caused by the app not being installed correctly or the admin service not being present in the system. Either way, the recommendation is to check for the presence of the admin in the device, and rerunning the installer if it is not present.
- This installer error:
  ![SecureUSB error](./img/XiaomiSecureUSBDisabled)
  Has appeared only in chinese brand devices, like Xiaomi, and can be fixed by enabling the Secure USB Install setting in developer options. <!---TODO-->
- Otherwise, _c_ ...
- These are placeholders for real troubleshooting steps, please excuse me while compiling them into a comprehensive list.
