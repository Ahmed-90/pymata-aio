![logo](https://raw.github.com/MrYsLab/pymata-aio/master/documentation/images/logo.png)
======
##pymata_aio is a high performance, non-blocking, Python asyncio client for the Firmata Protocol that supports the complete StandardFirmata protocol.

[![Join the chat at https://gitter.im/MrYsLab/pymata-aio](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/MrYsLab/pymata-aio?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

##Changes From Verion 2.16 to 2.17

* Licensing changed from GPL V3 to GPL Affero V3
* Callbacks now report pin type. See [this wiki page](https://github.com/MrYsLab/pymata-aio/wiki/Digital-And-Analog-Data-Reporting-Callback--Usage-Guidelines)
for details. __*Note this should not be a breaking change.*__ All existing applications should be able to run without
modification.



##Major features

* __Python 3.5+__ compatible.
    * **Implements [PEP 492](https://www.python.org/dev/peps/pep-0492/)**
    * **Applications developed with version 1.x of pymata_aio are backward compatible without modification.**
* **Implemented using the high efficiency Python [asyncio](https://docs.python.org/3/library/asyncio.html) library.**
* **Choose From 3 Included APIs**
     * **pymata_core** - a pure asyncio method call API.
     * **pymata3** - a pymata_aio plugin implementing a method call API that acts as a proxy for pymata_core. It shields the user from the details of the asyncio library.
     * **pymata_iot** - a pymata_aio plugin API that implements an [Autobahn](http://autobahn.ws/python/) Websocket server, and uses JSON messaging for application communication. 
          * After downloading and invoking **pymata_iot**, [**control your Arduino from a webpage!**](http://mryslab.github.io/pymata-aio/examples/uno_iot_tester.html)
* **Implements 100% of the StandardFirmata Protocol (StandardFirmata 2.5.3).**
* **Auto-detects Arduino COM ports.**
* **FirmataPlus (enhanced StandaradFirmata sketch) included with distribution. It adds support for:**
     * **HC-SRO4 Ultrasonic Distance Sensors using a single pin.**
     * **Stepper Motors.**
     * **Piezo Tone Generation.**
     * **2 Pin Rotary Encoder Support.**
* **FirmataPlusRB (enhanced StandaradFirmata sketch to control a [SparkFun Redbot](https://www.sparkfun.com/products/12649)) is included with the distribution. It adds support for:**
     * **Piezo Tone Generation.**
     * **Wheel encoders.**
     * **RedBot Accelerometer.**
     * **Check out [rbDashBoard](https://github.com/MrYsLab/rbDashBoard) for a web interface to the RedBot.**
     * **Check out [rb4s](https://github.com/MrYsLab/rb4s), a Scratch Program to control the RedBot.**
* **Ability to automatically capture and time-stamp user specified analog and digital transient input events on a per-pin basis.**
* **All 3 APIs support callback as well as a polled interface.**


__Detailed package information can be found on the [pymata_aio wiki](https://github.com/MrYsLab/pymata-aio/wiki).__

This project was developed with [Pycharm](https://www.jetbrains.com/pycharm/) ![logo](https://github.com/MrYsLab/python_banyan/blob/master/images/icon_PyCharm.png)
