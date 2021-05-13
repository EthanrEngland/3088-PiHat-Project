# 3088-PiHat-Project
UPS uHAT Design Concept 

This design project aims to detail a design of a microPi HAT (uHAT) compliant PCB of an uninterrupted power supply (UPS) “daughter board” for a Raspberry Pi (RPi) Zero single board computer (SBC). The uHAT is made up of several submodules that enable it to provide power to a RPi Zero when there is no power being supplied to the RPi by the mains power supply. 

The use cases are related to the common practice of setting up a RPi as a home server, network attached storage (NAS) system, as part of an arrangement with RPi add-ons with mobility for example a home-surveillance or a dash-cam camera system and general physical computing tasks with breadboards and software.  

The UPS uHAT will attach directly to (below / underneath) the RPi Zero with all RPi input/output (I/O) access points still available. The UPS uHAT will be affixed and will connect to the RPI via the bottom of certain general-purpose I/O (GPIO) pins on the RPi. The scenario this UPS uHAT will be used in is when there is loss of mains power and the RPi Zero device or system must either continue operating or have enough power to shutdown correctly. 

UPS uHAT Design Use Cases:

Scenario 1: RPi Zero user is a student needing to save work on a self-hosted data Syncthing server during load-shedding or a no-power event. 

A student hosts a data server for his work with Syncthing via a RPi Zero. The student has multiple machines: a desktop computer for when he is at his home, capable of fulfilling the high-end computing tasks he is required to perform (rendering on Blender), a laptop for use away from his desk and a tablet for annotating and note taking. The student needs all these machines to have all his work up to date with additions and edits collectively.  

The system used by the student involves using a RPi Zero with decent storage running Raspberry Pi OS that constantly hosts the Syncthing server and is connected to all the devices. The same work directories are shared across all devices. When a device is used to edit or add something to the work directories the mesh synchronizes each change across all devices. This ensures that the student can work at his desk or anywhere without having to move files around and keep track of changes manually. The RPi server also connects the devices to a set of external drives forming a NAS with large storage space to save large project directories. 

The student thus requires the RPi server to be running constantly. If there is a power outage, the student can still work using the portable and mobile devices but does not want the desktop (or battery flat devices) to go out of sync with each other.  

In addition, the RPi microSD storage device and that of the NAS system is safe from potential harm inflicted by sudden power off, most likely during operational status. 

The user designing a small, inexpensive UPS uHAT could solve this problem by providing power to the RPi server during the period that the student wishes to work whilst there is a power outage and or for the server to power off correctly. 

Specific user requirements: 

R1.1: UPS uHAT needs to provide power to the RPi from battery pack for up to 150 minutes. (R11 extension – larger battery pack needed) 

R1.2: The UPS uHAT must act as a no-break UPS. 

R1.3: The uHAT must be able to communicate to the RPi to power off when battery level falls below a certain level. (R13 / R14) 

 

Scenario 2: RPi Zero user with a home-surveillance setup (powered via ethernet) using camera modules on a set of RPi Zeros needing backup power during power outage events. 

A certain user has the need to power a surveillance system setup during no power events. The surveillance system in their household acts as a primary deterrent and defense measure against intruders. The user has designed camera modules using RPi Zero camera add-ons and 3D printing schematics of a housing to mount the camera modules in strategic positions around the residence. The cameras are all connected to the home network and are powered using long ethernet cables. The cameras alert the user using messages on a mobile device if certain motion parameters are met at certain times. 

It is imperative for this user that these camera modules continue to function during power outages. The user needs these cameras to function independently and as a system in order to better protect their home and their family. The design of a uHAT UPS add-on to the camera modules will solve the power outage problem should they provide power to each camera module while there is no mains power supply during the entire no power event. 

Specific user requirements: 

R2.1: UPS uHAT needs to provide power to the RPi from battery pack for up to 150 minutes. (R11 extension – larger battery pack needed) 

R2.2: The UPS uHAT must act as a no-break UPS. 

R2.3: The uHAT must be able to communicate to the RPi to power off when battery level falls below a certain level. (R13 / R14) 

 

Scenario 3: RPi Zero user that uses a generator system to power their essential devices during power outages. The user performs important physical computing tests and builds using RPi Zeros. The user needs a backup power reserve for the latency period when the mains power is removed, and the generator power is then used.  

A user is performing some important physical computing tasks as a freelance electronics engineer. The user has an assortment of RPi Zero devices connected to various test circuits and peripherals and machines over the network. When there is a power outage this user still needs to work and certain processes in his work should not be interrupted by a sudden outage. 

The user has a generator system for the essential appliances and his larger computing machines; however, he does not have a reliable switch system from mains power to generator power. Typically, he will check the load shedding schedule and turn on the generator just before the power goes off in order to remove the latency period between mains power usage and using the generator. This does not work when the user is not at home, is inattentive, when the load shedding schedule changes suddenly or during power outage events. 

The user can design a UPS uHAT that can power the device or device system immediately upon losing mains power. These uHATs can power the various devices until battery power is finished, then switch to generator power until mains power returns. Thus, the user can continue work through any power outage event and or perhaps when there is no generator fuel. 

Specific user requirements: 

R3.1: UPS uHAT needs to provide power to the RPi from battery pack for up to 150 minutes. (R11 extension – larger battery pack needed) 

R3.2: The UPS uHAT must act as a no-break UPS. 

R3.3: The uHAT must be able to communicate to the RPi to power off when battery level falls below a certain level. (R13 / R14) 
