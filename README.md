SystemKit
=========

A macOS system library in Swift based off of
[libtop](http://www.opensource.apple.com/source/top/top-100.1.2/libtop.c), from
Apple's top implementation.

### What's New

- ✅ **Support for Swift 6** added on *October 30, 2025*
- ✅ **Updated for macOS 26.0.1** compatibility
- ✅ **Updated for Xcode 26.0.1** compatibility

### Requirements

- [Xcode 15.3](https://developer.apple.com/xcode/downloads/)
- macOS 13.5 Ventura+
    - This is due to Swift
- Swift 6 (for latest version)

### Installation

#### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks.

You can install Carthage with [Homebrew](http://brew.sh) using the following command:

    $ brew update
    $ brew install carthage

To integrate SystemKit into your Xcode project using Carthage, specify it in your Cartfile:

    github "getangar/SystemKit"

Run `carthage update` to build the framework and drag the built SystemKit.framework into your Xcode project.
Don't forget to alter your Carthage [building phase for macOS](https://github.com/Carthage/Carthage#if-youre-building-for-os-x).

### Example

Sample output from
[example](https://github.com/getangar/SystemKit/blob/master/Example/main.swift).

```
// MACHINE STATUS

-- CPU --
	PHYSICAL CORES:  14
	LOGICAL CORES:   14
	SYSTEM:          2%
	USER:            4%
	IDLE:            93%
	NICE:            0%

-- MEMORY --
	PHYSICAL SIZE:   64.0GB
	FREE:            9.11GB
	WIRED:           3.68GB
	ACTIVE:          26.08GB
	INACTIVE:        24.08GB
	COMPRESSED:      306MB

-- SYSTEM --
	MODEL:           Mac16,11
	UPTIME:          5d 10h 40m 45s
	PROCESSES:       873
	THREADS:         4728
	LOAD AVERAGE:    [2.64, 2.46, 2.15]
	MACH FACTOR:     [10.897, 11.464, 11.43]

-- POWER --
ERROR - Example/System.swift:CPUPowerLimit() - kern_result_t = -536870160
	CPU SPEED LIMIT: -1.0%
	CPUs AVAILABLE:  -1
	SCHEDULER LIMIT: -1.0%
	THERMAL LEVEL:   Not Published

-- BATTERY --
	AC POWERED:      true
	CHARGED:         false
	CHARGING:        false
	CHARGE:          nan%
	CAPACITY:        0 mAh
	MAX CAPACITY:    0 mAh
	DESGIN CAPACITY: 0 mAh
	CYCLES:          0
	MAX CYCLES:      0
	TEMPERATURE:     0.0°C
	TIME REMAINING:  0:00
Program ended with exit code: 0
```


### References

- [top](http://www.opensource.apple.com/source/top/)
- [hostinfo](http://www.opensource.apple.com/source/system_cmds/)
- [vm_stat](http://www.opensource.apple.com/source/system_cmds/)
- [PowerManagement](http://www.opensource.apple.com/source/PowerManagement/)
- iStat Pro


### License

This project is under the **MIT License**.
