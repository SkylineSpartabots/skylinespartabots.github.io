---
title: Organization
---
# Organization
{:.no_toc}

{::options parse_block_html="true" /}
<div id="toc_nav" class="affix">
* This line is for the table of contents to be generated
{:toc}
{:.nav}
</div>
{::options parse_block_html="false" /}

<!-- Don't change anything above this point! -->

## Introduction

We, like many robotics teams, use an organizational pattern called command-based programming. Our robot code is split among:
- `Robot.java`
- `RobotMap.java`
- `OI.java`
- commands
- subsystems

For example, this is structure of the [YogaBallBot code][YogaBallBot-repo]:

```
├───commands
│   ├───DriveWithJoystick.java
│   ├───MoveArm.java
│   ├───RollIn.java
│   └───RollOut.java
├───subsystems
│   ├───Arm.java
│   ├───DriveTrain.java
│   └───Roller.java
├───OI.java
├───Robot.java
└───RobotMap.java
```

## RobotMap.java
This creates global integers telling you where each input is. These integers are the values of the port numbers and are used when setting an object to a port.

## Command-based
There are two categories extremely important to command-based programming: subsystems and commands.
Subsystems are classes that correspond to an actual smaller system of the robot's hardware. A drive train, an elevator, a shooter, and a claw are examples of subsystems. Commands are like demands for a subsystem to do something specifically. For example, drive forward, raise elevator, shoot balls, and close claw are examples of commands. Commands run either when scheduled or in response to a button press.

## Subsystems
Each subsystem has a constructor and these methods:
- `public void initDefaultCommand()`
  - Sets the command which is scheduled whenever the subsystem is idle (the command currently requiring the system completes).
  - Usually empty for most subsystems.
  - If the subsystem is the drive train, it has something like `setDefaultCommand(new DriveWithJoysticks());`

## Commands
Each subsystem has a constructor and these methods:
- `protected void initalize()`
	- Is called the first time this command's instance runs.
- `protected void execute()`
	- Is called repeatedly by the scheduler.
	- Usually only non-empty if this command runs constantly or when the button is held.
- `protected boolean isFinished()`
	- Is called repeatedly after `execute()`
	- Should return `true` once the command does not need to run anymore and `false` otherwise.
	- Usually always returns true **if** this command is run on a button press and not a hold.
- `protected void end()`
	- Is called once if `isFinished()` returns `true`.
- `protected void interrupted()`
	- Is called if another command has been scheduled that requires the same subsystem(s) that this command requires.
	- Usually contains just this one line: `end();`

### Command groups
Command groups are complex commands made from a sequence of simpler commands. You can specify the commands to run in some order, with some commands either running at the same time (parallel) or one after the other (sequential).

It is very common for autonomous routines to use command groups to execute a complex series of tasks.

## Git
Git is a distributed version control system. GitHub is a website and a free service that hosts git stuff so that people can collaborate on projects. Projects are called repositories. So each of Spartabots' code projects is in a repository. GitHub puts them all in our organization: [SkylineSpartabots](https://github.com/SkylineSpartabots).

Reasons we use Git:
- organization
- history (so we can revert changes and track progress)
- cooperation (multiple people can work on the same code

[YogaBallBot-repo]: https://github.com/SkylineSpartabots/YogaBallBot
