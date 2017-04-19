# Connectivity

## Configuring the radio
[Configuring the radio (docx)](https://docs.google.com/viewer?a=v&pid=sites&srcid=ZGVmYXVsdGRvbWFpbnxzcGFydGFib3Rzd2lraXxneDo1MjVkNTY4YTcxZjhkOTY1)

## Imaging the roboRIO
[Imaging the roboRIO (docx)](https://docs.google.com/viewer?a=v&pid=sites&srcid=ZGVmYXVsdGRvbWFpbnxzcGFydGFib3Rzd2lraXxneDoxYzEzMjZlY2IwOGNkODgz)

## Connecting to the roboRIO
### How to connect
1. Connect your computer to the roboRIO's USB A port
2. Go to command prompt and run `ping 172.22.11.2`
	- If the ping doesn't work:
		- Make sure the robot is turned on and powered
		- Ensure that you are connected via USB
		- Try a different computer
3. Go to the address 172.22.11.2 in Firefox (or IE)
	- Click "Tap here to active plugin" if Firefox blocked Silverlight from running
4. Once the webpage loads, you should see something like this:
![Screenshot of NI Configuration Homepage](https://cloud.githubusercontent.com/assets/14433542/17985907/04974504-6acd-11e6-8c5c-58e3f22313bd.png)

### Useful links
[Docs](https://wpilib.screenstepslive.com/s/4485/m/13503/l/242608-roborio-networking)

[Troubleshooting](https://wpilib.screenstepslive.com/s/4485/m/24193/l/284355-roborio-network-troubleshooting)

## Configuring CANTalon
### Connect computer to roboRIO
1. Connect your computer to the roboRIO's USB A port
2. Go to command prompt and run `ping 172.22.11.2`
	- If the ping doesn't work:
		- Make sure the robot is turned on and powered
		- Ensure that you are connected via USB
		- Try a different computer
3. Go to the address 172.22.11.2 in Firefox (or IE)
	- Click "Tap here to active plugin" if Firefox blocked Silverlight from running
4. Once the webpage loads, you should see something like this:
![Screenshot of NI Configuration Homepage](https://cloud.githubusercontent.com/assets/14433542/17985907/04974504-6acd-11e6-8c5c-58e3f22313bd.png)

### Connect CANTalon
1. If the CANTalon is new:
  - Strip the ends of the large red and black wires.
  - Strip the ends of the small yellow and green wires.
2. Connect the red wire to a red port and the black wire to a black port on the Power Distribution Board.
![Power Distribution Board](https://cloud.githubusercontent.com/assets/14433542/21759146/e404bc50-d5f6-11e6-8974-924da38c6d6f.png)
3. Connect the yellow and green wires to the CAN extenders near the roboRIO.

![CAN ports](https://cloud.githubusercontent.com/assets/14433542/21833262/ca7b4e96-d765-11e6-8a84-d4049bdec52e.png)

4. On the NI Configuration homepage, click the Talon SRX with Device ID 0 (default for new CANTalons) or another number.
5. Click the "Light Device LED" and click "Save" and check that the CANTalon's lights are blinking rapidly.
6. If you need to change the Device ID, set the Device ID to something other than 0 and click "Save". Remember that no two devices should be connected that have the same Device ID.

### Useful links
[Docs](https://wpilib.screenstepslive.com/s/4485/m/13503/l/242608-roborio-networking)

[Troubleshooting](https://wpilib.screenstepslive.com/s/4485/m/24193/l/284355-roborio-network-troubleshooting)
