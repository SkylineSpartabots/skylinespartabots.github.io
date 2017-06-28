---
title: Connecting to the roboRIO
---
# Connecting to the roboRIO
{:.no_toc}

{::options parse_block_html="true" /}
<div id="toc_nav" class="affix">
* This line is for the table of contents to be generated
{:toc}
{:.nav}
</div>
{::options parse_block_html="false" /}

<!-- Don't change anything above this point! -->

## How to connect
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

## Useful links
[Docs](https://wpilib.screenstepslive.com/s/4485/m/13503/l/242608-roborio-networking)

[Troubleshooting](https://wpilib.screenstepslive.com/s/4485/m/24193/l/284355-roborio-network-troubleshooting)
