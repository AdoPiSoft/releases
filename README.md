4.0.0-beta.8
===================

* Fix device status still connected after reboot even if no running session
  - This is only a bug in admin display, the device is not really connected to internet and the status in portal is actually disconnected.

* Fix  bad gateway error caused by socket.io error

* Can add device manually



4.0.0-beta.7
===================

* Auto select coinslot if machine has single coinslot

* Changes to wifi user status idle/active indicator:
  - GREEN = Active
  - ORANGE = Idle

* Can buy E-Load in portal

* Can backup and restore settings from version 4.0.0-beta.7

* Fix wireless coinslot connect/disconnect loop which also causes bad gateway error
  - Please **[download](http://wiki.adopisoft.com/doku.php?id=4.0.0-beta.1:index#wireless_coinslot)** the latest binary for your wireless coinslots

4.0.0-beta.6
===================

* Fix network traffic graph not working

* Fix race condition of starting device sessions

* Fix sales inventory

* Separate sales by coinslot

* Fix captive portal not opening automatically when device has no session

4.0.0-beta.5
===================

* Fix device status is "disconnected" even if it has running session after reboot

* Show device active status by color.
  - GREEN = Active (device is using internet)
  - GRAY = Device is idle (no network traffic) or may not be connected to wifi/LAN
  - Status will reflect within 10 to 15 seconds interval

* Include crash error (bad gateway) in system logs

* Set correct timezone on boot.
	 - If you find that your sales inventory is empty, it is because previous timezone was not set correctly and may have been saved using different timezone.

* Fix errors when pausing session with multiple users and other users are not online

4.0.0-beta.4
===================

* Fix device with multiple sessions not disconnected when cleared from admin

* Added coinslot relay delay option

* Fix voucher CSV spacing


* Restore settings from old version (3.0.8x) to version 4
  - Banners
  - Logo
  - Timer & Rates Setings
  - Bandwidth Settings
  - Captive Portal Settings

4.0.0-beta.3
===================

* Fix major bug when user has multiple session


4.0.0-beta.2
===================

* Fix enable/disable SSH not permanent

* Fix unable to disable built-in wifi

* Can restore old backup from v3.0.8x
  - Only customer's remaining time and vouchers are restored for now. Bandwidth settings, rates, logo and bannerse cannot be restored yet. (work in progress)
  - Backup from v4.0.0-beta.1 is not yet compatible with v4.0.0-beta.2 (work in progress)

* Fix device not disconnected when session is cleared from admin

* Fix fetching github releases
