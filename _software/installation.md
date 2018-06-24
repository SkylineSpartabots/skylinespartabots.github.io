---
title: Installation
---
# Installation
{:.no_toc}

{::options parse_block_html="true" /}
<div id="toc_nav" class="affix">
* This line is for the table of contents to be generated
{:toc}
{:.nav}
</div>
{::options parse_block_html="false" /}

<!-- Don't change anything above this point! -->

## What to install
To develop and deploy Java code for FRC robots, you need:
- Eclipse
- Java Development Kit (JDK)
- WPILib Java plugins for Eclipse
- FRC Update Suite
- CTRE plugins (for CAN Talons)
- navX-MXP plugins
- Some Git client (to collaborate on GitHub repos)

**Note:** In order to deploy code to the robot, you must use FRC's Driver Station software, which only runs on Windows computers. You can still write code on Eclipse on Mac OSX and Linux and pull/push to GitHub.

**Note:** **There is another IDE (IntelliJ) that you can use for FRC:** [Installing IntelliJ IDEA with WPILib (external link)](https://gitlab.com/Javaru/frc-intellij-idea-plugin/wikis/home)

## Eclipse, JDK, and WPILib plugins
[Official instructions](https://wpilib.screenstepslive.com/s/currentCS/m/java/l/599681-installing-eclipse-c-java)

**Notes:**
- We strongly recommend downloading Eclipse Oxygen, the newest version.
- Skip the "Installing C++ Toolchains (C++ teams only)" and the "Adding C++ to Java Eclipse" sections
- We recommend "Option 1: Online Install" for installing the development plugins

## FRC Update Suite
[Official instructions](https://wpilib.screenstepslive.com/s/currentCS/m/java/l/599671-installing-the-frc-update-suite-all-languages)

**Notes:**
- Make sure you fully uninstall old versions of National Instruments software before updating
- The decryption key from the Kickoff broadcast is `pLaY&4%R3aL!`
- For "Organization," enter "Skyline Spartabots"
- You can find our team's serial number on our Discord

## CTRE plugins
[Installer link](http://www.ctr-electronics.com/control-system/hro.html#product_tabs_technical_resources)

Download "CTRE Phoenix Framework Installer (.zip)" and extract the folder. Run the installer and follow the directions given by the installation wizard.

In the "Select components to install" section, you don't need to check the "LabVIEW" or "HERO C#" components because our club doesn't use them.

[Troubleshooting](https://www.ctr-electronics.com/downloads/pdf/CTRE%20Toolsuite%20Installation%20Guide.pdf)

## navX-MXP
The navX-MXP is a gyroscope/accelerometer/compass that we attach to our roboRIO for direction.
[KauaiLab's tutorial](https://www.pdocs.kauailabs.com/navx-mxp/software/roborio-libraries/java/).

**Note:** Skyline High School's Wi-Fi network sometimes blocks this website because of file-sharing content, so you may need to download the navX libraries at home.

## Git clients
There are many Git clients that work perfectly well. It's important that you choose one that you understand how to use. These are some of the Git programs that our team members use:
- [git-scm](https://git-scm.com/downloads) (Command line and barebones GUI)
- [GitHub Desktop](https://desktop.github.com/) (GUI only)
- [GitKraken](https://www.gitkraken.com) (GUI only)
- [SourceTree](https://www.sourcetreeapp.com/) (GUI only)

Here is a more complete [list of Git clients](https://git-scm.com/downloads/guis).
