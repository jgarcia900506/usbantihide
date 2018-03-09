Project:      USB_AntiHide
Author:       Juan Pablo Garcia Rivera
Ver.:         1.0
Company:      A&Dev
Email:        j.garcia900506@gmail.com
Web:          http://jgarcia.my-place.us
Description:  Find usb storage devices and execute own batch scripts

USE
Download project on "C:\USB_AntiHide" and execute core.exe

AUTORUN CONFIGURATION FOR Win7 Original
Execute this command on admin console:

SchTasks /create /tn USBAntiHide /tr C:\USB_AntiHide\core.exe /sc ONEVENT /ec Microsoft-Windows-DriverFrameworks-UserMode/Operational /mo "*[System[Provider[@Name='Microsoft-Windows-DriverFrameworks-UserMode'] and EventID=2101]]"
