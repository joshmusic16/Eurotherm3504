# Eurotherm3504
3504 Eurotherm power supply automation via LabVIEW.
This code, which is adapted from Eurotherm code, is capable of monitoring the given process variable (temperature of evaporator) thorugh MODBUS communication. 
The goal temperature can be reached by a slow increase of PV over a set amount of time, so as not to quickly heat up the evaporator, which can lead to rapid 
thermal expansion of the filament, which can lead to a broken filament. Once the goal temperture is reached, the program stalls for a set amount of time to allow
deposition from the evaporator, and then the PV is slowly lowered until the filament reaches room temperture. 
The MODBUS communication is initiated by VISA controls via LabVIEW and is physically connected by a 9 pin DB9 cable (in our case through USB conversion).
