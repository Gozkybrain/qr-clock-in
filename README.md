# QR Scan to Clock In System
This is a simple attempt to create a Clock In system for employees using QR Scan. The database is handled by firebase, the whole process is quite simple and straightforward.

## How to Use
There is a Login and Registration Page used to handle authentication.

On registration, the information of the device is stored for the user on the database. 

On the Scan Clock In page, if the user's device does not match the info on the database then there would not be a clock in. This will assist employers so that someone else does not clock in for just anyone.

If the device matches, then the user gets clocked in and their ip, and time is sent to the database as last clocked it.

This will enable the admin of the firm view when all employees clock in from his panel. With the ip updated, then he can compare if they actually signed in from anywhere around the office as the office ip will be made available.


## Routes
* `/login and /register:` The login and register routes are used for authentication. All employee accounts must be registered and paired to a device ID, this way someone else can not clock-in for an employee. Clocking employee must be logged in to actually clock in and update their information.

* `/admin:` The employer or HR can view all the users, and their last clocked in dates & time, the user's clocked in ip, and device id.

You actually need two devices to test this system, by scanning with another device. On the other hand, you can print the page and scan.
