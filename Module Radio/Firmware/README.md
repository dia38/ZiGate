# Version 3.0e

* Add Private cluster 0xFC01 to manage some Legrand Netatmo stuff
* Add Power configuration Cluster. Used by Ikea . https://github.com/KiwiHC16/Abeille/issues/139
* Add 0xFF02 Cluster. Used by Xiaomi devices for battery informations. https://github.com/KiwiHC16/Abeille/issues/141
* Add TimeServer functions (Set 0x0016 and Get 0x0017). You can give a datetime to ZiGate. Some device tell ZiGate to get datetime like some Xiaomi devices.
* Fix UART control flow.
* Fix Device announce from some devices. Ex : fix the Legrand Netatmo join sequence.
* Update Device Timeout. 256 min to 16384 min. Limit Xiaomi devices lost. Not a fix but should be better. Not really tested in real condition. https://github.com/fairecasoimeme/ZiGate/issues/38

# Version 3.0d

Warning !!! you have to erase EEPROM or PDM. the memory structure must be regenerated.

* Fix max number group table to 5.  https://github.com/KiwiHC16/Abeille/issues/80
* Fix wrong output cluster count and attributes. https://github.com/fairecasoimeme/ZiGate/issues/18
* Add Short Address to 0x8062 / Get Group. https://github.com/fairecasoimeme/ZiGate/issues/19
* Add new command 0x0009 / 0x8009 --> NetworkState. Give network State. https://github.com/fairecasoimeme/ZiGate/issues/15

# Version 3.0c

* Fix Attributes Data conversion uint32. Real and true value from consumption data device
* Fix Get Xiaomi private data from cluster 0x0000 attributes 0xFF01 with specific manufacturer 0x115F

# Version 3.0b

* Up to 80 devices. 50 ZiGate's children and 30 others devices linked to routers
* Add new command. 0x015 (Get Devices List) and 0x8015 for the response. More details on http://zigate.fr/wiki/commandes-zigate/
* Fix other minor bugs and enhancements

# Version 3.0a

 * Change max number controled devices to 60
 * Fix some bugs

# Version 3.0

 * Add Orvibo ZigBee material compatibility (Device 0x0A)
 * Add Pressure measurement management (Xiaomi aqara)
 * Add Analog input basic cluster management (Xiaomi aqara)
 * Add Multistate Input basic cluster management (Xiaomi aqara)
 * Add Quality Link on Input Message (To ZiGate) (see protocol section)
 * Configure default channel 11
 * Configure for JN5168-001-M05 (E_MODULE_JN5168_001_M05_ETSI) -- For Europe
 * Fix IAS management. Compatibility with old version
 * Fix multi-endpoint device compatibility (For example  Cube magic Xiaomi)
 * Fix private cluster management
 * Fix some bugs and add debugs

# Initial Version
JN-AN-1216-Zigbee-3-0-IoT-ControlBridge
