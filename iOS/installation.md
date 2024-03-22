# iOS Installation Guide

## Requirements

- iOS 15.0 and above, excluding version 15.1.
- The user's iCloud credentials should be accessible.
- No other MDM/VPN/DNS/Proxy profile on the device.
- On iPhones 8 and older, or any iOS device with a _Home Button_, it is required that it completely works.
- Charging port must work.
- Storage must not be completely full.
- On iOS 16.0 and above, the passcode must be disabled.
- A computer with iTunes installed.

## Warnings

- Music that is stored in the device that was transferred from a computer will be deleted from the device, so make sure to have it backed up.
- Apple wallet cards will be lost when removing the passcode, even if the iOS version does not require this, the process **_can_** still remove these.
- Shared Albums usually need to be added back into the device. To get them back, go to _Settings_ => _Photos_ and toggle off and back on Shared albums. They should appear on the phone, once again.
- Home Screen apps are usually rearranged after insatllation, they can be moved to their original arrangement afterwards.
- If the device has a Home Button, make sure that it works properly, as it is needed for those devices to be able to finish installing the filter.
> [!Warning]
> The virtual button from accessibility does not fulfill this requirement. If the phone has a physical home button, then that physical phone button must work.

## Step-by-step installation

- On the device, disable Find My, this requires the user's iCloud account credentials
- On [the portal](https://portal.mbsmartservices.net) select _Open Account_ or follow [this link](https://portal.mbsmartservices.net/mbsmart/Admin.html?data=main&content=ioscreate) to create a new account, fill out the linkcode, a security pin, and the user's info. Have the customer read and accept the terms & services, then click submit.
- Open the installer via TAG Hub, and log in with your credentials (for TAG it is always the same as the admin.tag.org ones).
- Select wether you would like for the device to be backed up to the computer or not (generally not needed and can take a really long time).
- From the portal, copy and paste the generated ID into the field named _Paired Device ID_.
- Check _Disable MDM Removal_.
- Click _Proceed_.
- On the device, after it reboots, swipe up (or in older models, press the home button) to continue, and accept the profile download.
