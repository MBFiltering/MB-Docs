# Android Installation Guide


## Requirements:

- Android version 5.0 and above
- No other device owner present in the device
- Storage must not be completely full
- Charging port must work (unless the idea is to install via QR code)
- Secondary Users such as Guest User, Multiple Users or Dual Messenger will cause the installation to fail, as such, these need to be removed as well.

## Brand Specific Instructions:

### Samsung

- _Secure Folder_ causes issues with installation, where the app is not able to be installed correctly onto the device, thus uninstalling it from settings is necessary before installing the filter by entering into _Secure Folder_ => _Settings_ and pressing uninstall.

### Xiaomi

> [!Note]
> There are branches of Xiaomi which also make phones which have similar instructions, like Poco and Redmi.
- It is required to disable _MIUI Optimization_ in developer options and enable _Install via USB_ in the USB debugging section

### Other Chinese Brands

- Like with Xiaomi, _Install via USB_ needs to be enabled in Developer Options
- Some additional permissions might be required for background apps, so set MB Smart to have them allowed

## Step by Step installation:

- Go into _Settings_ => _About phone_[^1] => _Software Information_.
- Scroll down to _Build number_ and tap until a notice appears informing that developer options have been enabled.
- Go back to the main settings menu, where a new option called _Developer options_ ahould have appeared.
- Go into _Developer options_, scroll down to _USB debugging_ and enable it.
- On the computer, open the installer, either [standalone](https://installer.mbsmart.net/MB_Installer.exe) or through TAG Hub and connect the device via USB.
- Accept the connection on the device, the installer should then go through several screens and then complete, showing a green screen[^2].
- On the device, the application should have installed and started on it's own, accept the terms and conditions to continue.
- Continue to account creation, fill in the user's details, the office linkcode, and a pin which will be used for support requests.
- Once account creation is done, you will be prompted to give permissions to the MB Smart app.
- A payment screen will be presented, after which you will proceed to configure the device on the portal, optionally.

### QR Code Method:

> [!Note]
> This is only available for devices which are not provisioned (check in the Device Owner section to find out about provisioning), are running Android version 7.0+ and have a QR code reader. It will not work otherwise.
- Turn on a new or factory-reset device.
- Tap screen 6 times in the same spot. This triggers the device to prompt you to scan a QR code.
- Scan this QR code: ![QR Code](./img/QRcode.jpg)

## Transferring to a new device while keeping the same account:

- Uninstall filter from the old device. If this is not possible, it will not cause issues.
- On the [portal](https://portal.mbsmartservices.com), after filter is set to **_off_** on the Main tab, a RecoveryID will be generated. This can be found on the User list, on the last row. ![You can find it on the rightmost column of the User list](./img/RecoveryID.png)
- Install on the new device normally up until getting a green screen on the installer, and proceed into the device.
- Instead of creating a new account on the device, select Recover and insert the RecoveryID generated, including the colon and email, the format should be <#ID:email\>
> [!Note]
> Most keyboards insert spaces after punctuation, so be mindful of this and make sure there are no spaces around or in between the RecoveryID parts
- Set up permissions as you would do any other installation. The filter should now be completely installed and configured the same as the original account was.
> [!Important]
> A new ID will be generated for the new device, so if there is need to work on the portal for the account make sure to use the appropiate one.

## Compatibility notes & Known issues:

- Android GO versions 5.0 and above are compatible as well.
- Samsung S6, S7 and S8 devices are likely to encounter a bug where a passcode is set on the device unintentionally, with no known solution other than doing a Factory Reset, recommendation is to not install on these devices at all.
- Some chinese can display accessibility issues, in this case we recommend avoiding _Bypass(IAB Blocked)_ as much as possible.
- On Android 9 it is possible that the Chrome and Google apps will not be filtered. In these situations it is recommended to close them or, for Chrome only, set the app to be whitelisted. The best solution is to update to Android 10+.
- On some Motorola devices, we have seen an issue where battery charging is limited to 30%, only solution known is to remove the Device Owner.
- Oppo and Realme brand devices have not been succesfuly installed on. (Please contact if this is proven to be untrue, with details.)
- We have seen mixed success with the Unihertz Jelly 2.
- Amazon Fire devices, even though running a version of Android, are not compatible.

### TAG policy notes:

- CAT S22 Flip devices have some issues with permissions being missing, among other compatibility issues. TAG policy is not to install on these devices.
- Xiaomi F21 (sometimes known as Duo Qin F21) devices are not well supported by the filter, and can have some issues. TAG policy is not to install on these.
- MP3 players are against TAG policy.

## Device Owner:

- A device owner app is a special device admin that cannot be deactivated by the user, once activated. It also cannot be uninstalled.
- A device owner provisioned device can have Android's full range of management policies.
- A device cannot have users or user data configured for provisioning to be supported.

### Provisioning

- A device is considered provisioned once a device owner, user or device admin is set up in the device.
- A device can be deprovisioned manually by removing all accounts from settings or, alternatively, by factory-resetting it.

## [Users](https://source.android.com/docs/devices/admin/multi-user#categories_of_users):

- System user: the first user added to a device, which cannot be removed except for a factory reset and is always running even when other users are in the foreground. It has special privileges and settings only it can set.
- Headless system user: same as system user, but configured to run in headless mode. Always runs in background, and requires additional users in the foreground for enabling user interactin.
- Secondary user: any user added to the device other than the system user. These can be removed and cannot impact other users on the device. They can run in the background and continue to have network connectivity.
- Guest user: temporary secondary user, with the option to quickly discard when usefulness is over. Only one guest user is permitted at a time.
- Admin user: has permissions to create and remove other users, as well as control multi-user settings. By default, only the system user is an admin.

---

[^1]: Sometimes called by other names, if there is difficulty finding this section, just search for build number in the Settings app.
[^2]: Sometimes we encounter errors, refer to the Troubleshooting section for more info.
