# MB Smart Android Insallation Troubleshooting:

## Known installer error messages:

- These installer errors:

  ![DPM error of reinstalling while removal is in process](./img/BeingRemoved2.png)

  ![Regular error of owner being installed while removal is in progress](./img/ReinstallRemovalInProgress.png)
  Indicates that you are trying to install the filter while the device owner that was present
  is currently being removed, and waiting a minute or two would be recommended.

- This installer error:

  ![UnknownAdmin error](./img/UnknownAdmin.png)
  Indicates that the device admin was not recognized, which could be caused by the app not being
  installed correctly or the admin service not being present in the system.
  Either way, the recommendation is to check for the presence of the admin in the device,
  and rerunning the installer if it is not present.

- This installer error:

  ![SecureUSB error](./img/XiaomiSecureUSBDisabled.png)
  Has appeared only in chinese brand devices, like Xiaomi, and can be fixed by enabling the
  Secure USB Install setting in developer options. <!---TODO-->

- This installer error:

  ![Owner not set, profile owner already present](./img/ProfileOwnerSet.png)
  Means that the device already has a profile owner.
  If no profile owner can be found on the device, then the issue lies with the ROM and the device
  should be deemed incompatible with MB Smart (just this one, other devices of the same model
  might have an unaffected ROM).
  This error is mostly found on Qin devices.

- This installer error:

  ![ProvisioningPreCondition99 error](./img/ProvisionError99.png)
  Indicates that there are multiple users present on the device. This can be fixed by
  removing the extra users, in whatever form they exist on the particular device
  and rerunning the installer.

- This installer error:

  ![App did not install correctly](./img/appincorrect.png)  
   Could mean a number of things, but mainly that the installer considers the installation of the
  APK to have been unsuccessful. This might be incorrect, so please verify if the app is present
  in the device or not. If it is not present, please check if a _Secure Folder_ is present
  (or something akin to that) and remove it. If the app did install correctly,
  the installer should have an option to continue with the installation.

- Otherwise, _c_ ...
- These are placeholders for real troubleshooting steps, please excuse me while compiling them into a comprehensive list.
