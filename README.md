# QR Scan to Clock In System
This is a simple attempt to create a Clock In system for employees using QR Scan. The database is handled by firebase, the whole process is quite simple and straightforward.

## How to Use
There is a Login and Registration Page used to handle authentication.

On registration, the information of the device is stored for the user on the database. 

On the Scan Clock In page, if the user's device does not match the info on the database then there would not be a clock in. This will assist employers so that someone else does not clock in for just anyone.

If the device matches, then the user gets clocked in and their ip, and time is sent to the database as last clocked it.

This will enable the admin of the firm view when all employees clock in from his panel. With the ip updated, then he can compare if they actually signed in from anywhere around the office as the office ip will be made available.


