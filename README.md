# DWDMME-MIB
### DESCRIPTION
**DWDM.ME** MU Series Data Transmission Platform MIB file.

### CAUTION
* This MIB file was **REVERSE ENGINEERED** from a partial info provided by local DWDM.ME distributor and MU Series hardware output.
* This MIB file **CAN BE MODIFIED HARDLY** if vendor will provide additional information or i'll find unknown OIDs meanings.
* This MIB file **WAS NOT CHECKED** either by vendor, nor by vendor's representatives. At all.
* This means there **ARE** inaccuracies, omissions and errors. Anyway, it looks much better, then without this file.

**So shut up, grab it for free, use it on your own risk and don't complain - you've been warned!**

### EXAMPLES
* snmpwalk -M +mibs/dwdm.me -v2c -c XXX X.X.X.X DWDMME::products
```
DWDMME::sysName.0 = STRING: "MU-HOSTNAME"
DWDMME::sysLocation.0 = STRING: "555, Some str., Nowhere Town, NO"
DWDMME::sysContact.0 = STRING: "noc@nowhere.no"

...
```
* snmpwalk -M +mibs/dwdm.me -v2c -c XXX X.X.X.X DWDMME::nmsUnit

```Don't ask me why vendor placed PSU information in the NMS unit subtree - it looks as weird to me as it is to you, just live with this knowledge.```
```
DWDMME::nmsType.0 = STRING: "NMS"
DWDMME::nmsSoftwareVersion.0 = STRING: "5.60"
DWDMME::nmsDescription.0 = STRING: "DWDM Chassis :: NewTelco 1.1"
DWDMME::lan1Link.0 = INTEGER: up(1)
DWDMME::lan1Speed.0 = INTEGER: 100
DWDMME::lan2Link.0 = INTEGER: notLinked(0)
DWDMME::lan2Speed.0 = INTEGER: 10
DWDMME::lan3Link.0 = INTEGER: notLinked(0)
DWDMME::lan3Speed.0 = INTEGER: 10
DWDMME::lan4Link.0 = INTEGER: notLinked(0)
DWDMME::lan4Speed.0 = INTEGER: 10
DWDMME::sfp1Status.0 = INTEGER: 1
DWDMME::sfp1Link.0 = INTEGER: 1
DWDMME::sfp1Speed.0 = INTEGER: 103
DWDMME::sfp1Wavelength.0 = INTEGER: 1559
DWDMME::sfp1Fibermode.0 = INTEGER: 0
DWDMME::sfp1TransDistance.0 = INTEGER: 80
DWDMME::sfp1Temperature.0 = INTEGER: 3026
DWDMME::sfp1Voltage.0 = INTEGER: 327
DWDMME::sfp1Current.0 = INTEGER: 6602
DWDMME::sfp1RxPower.0 = INTEGER: -887
DWDMME::sfp1TxPower.0 = INTEGER: 291
DWDMME::sfp2Status.0 = INTEGER: 0
DWDMME::sfp2Link.0 = INTEGER: 0
DWDMME::sfp2Speed.0 = INTEGER: 0
DWDMME::sfp2Wavelength.0 = INTEGER: 0
DWDMME::sfp2Fibermode.0 = INTEGER: 0
DWDMME::sfp2TransDistance.0 = INTEGER: 0
DWDMME::sfp2Temperature.0 = INTEGER: 0
DWDMME::sfp2Voltage.0 = INTEGER: 0
DWDMME::sfp2Current.0 = INTEGER: 0
DWDMME::sfp2RxPower.0 = INTEGER: 0
DWDMME::sfp2TxPower.0 = INTEGER: 0
DWDMME::power1Type.0 = STRING: "CH20-PW-C"
DWDMME::power1Status.0 = INTEGER: up(1)
DWDMME::power2Type.0 = STRING: "CH20-PW-C"
DWDMME::power2Status.0 = INTEGER: up(1)

...
```
