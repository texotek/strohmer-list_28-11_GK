# Festo Automation Suite

The Festo Automation Suite is a tool for operating festo robotic parts and related parts from
related companies. It provides a integrated development environment for easy configuration and programming.

## 1. Seting up devices

For setting up parts and devices using the Festo Automation Suite:

1. Go to the topology overview
2. Add a new device

Now it will go into a guided setup mode, where you can enter a part identifier that is present on your part that you want to add.

You can find the part indentifier in this format for example:

`CEMMS-AS-70-M-LS-RM` 

or you can enter a part number that looks like this:

`550119 `

## 2. Guided Setup

Thankfully the festo automation suit integrates multiple parts.
The IDE can calculate how to operate the parts in low level, without user intervention.

When adding a motor controller such as the `CMMT-AS-C2-3A-EC-S1`, when you click `Open Plugin`,
you see a window with `Start First Setup` and `Manual Setup`.

`Start First Setup` provides a guided setup.

When you click that window it opens a interface where you can configure the parts which the motor is connected to.

In this example we have the 

1. Motor
2. Axis
3. Mouting Kit
4. Gear

we can configure.

### 2.1 Device Settings
In the device settings we can specify detailed configuration that applies to our use case.

Mains Voltage is the Voltag supply apply to the device.

We can enable the Drive via:

1. IO (Direct IO on Controller with voltage)
2. Fieldbus
3. Plug-in (Festo Software)


### 2.2 Component Settings
For each component in the Device you can configure Application Data, Hardware Switches, Mounting Method and Software Limits.

Here you must look at the individual components and your Application to see what you have to enter into the data.

## 3. Connecting the devices

To connect the devices to each other with an ETHERCAT Bus you have
to drag and the connection line to the appropiate Ports.

There may be ip address collisions you have to set the addresses in the Plug In editor for each device correctly.

192.168.42.110-14

## 4.Programming with CODESYS

Soft motion