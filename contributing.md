---
title: Contributing
---
# Contributing
This is how _you_ can help improve the Spartabots Wiki:
- make articles more coherent and readable
- add missing information
- correct errors and typos
- update articles with new information

## Get a GitHub account and access to this repository
1. Sign up for a GitHub account at [github.com](https://github.com/join).
    - If your username doesn’t contain your name, then put your real name in your profile so that other robotics members can identify you more easily.
2. If you are a member of Skyline Robotics, request to join the [Spartabots organization](https://github.com/SkylineSpartabots) on GitHub. We will accept your request pretty quickly and give you access to this repository.
3. If you are not a member of Skyline Robotics, fork this wiki's repository and submit a pull request with any changes.

## Learn Markdown
You can learn how to use GitHub Flavored Markdown [on GitHub's help page](https://help.github.com/articles/about-writing-and-formatting-on-github/).

In addition, there are a few specific formatting features on this wiki:

| Style | Syntax | Example | Output |
| :--- | :--- | :--- | :--- |
| Green text (good) | `<span class="good">...</span>` | `<span class="good">indents > spaces</span>` | <span class="good">indents > spaces</span> |
| Strikethrough red text (bad) | `<span class="bad">...</span>` | `<span class="bad">spaces > indents</span>` | <span class="bad">spaces > indents</span> |
| Bolded and underlined red text (safety) | `<span class="safety">...</span>` | `<span class="safety">Safety</span>` | <span class="safety">Safety</span> |
| Flashing rainbow text (important) | `<span class="important">...</span>` | `<span class="important">IMPORTANT</span>` | <span class="important">IMPORTANT</span> |

## Make a change
Our file structure of Markdown files (end in .md) looks like this, not including the index.md files:
```
├───_build
│   ├───design.md
|   ├───electronics.md
|   ├───parts.md
|   └───tools.md
├───_software
|   ├───connectivity
|   |   ├───configuring-the-radio.md
|   |   ├───imaging-the-roborio.md
|   |   ├───connecting-to-the-roborio.md
|   |   └───configuring-cantalon.md
│   ├───installation.md
│   ├───organization.md
│   └───java.md
├───contributing.md   # this page
└───README.md         # the home page
```
You can edit any of these files, but please ask before creating a new page.

## Review your change
Before committing, ask yourself these questions:
1. Are there any grammar errors or spelling mistakes?
2. Are there enough pictures or screenshots to explain?
    - Pictures and diagrams for hardware
    - Screenshots and wiring diagrams for software
3. Is the page formatted nicely?
    - Bolded key phrases
    - Information in paragraphs
    - Easy-to-scan lists

## Commit/Push your change
**Make sure** your commit message follows these guidelines:
1. Short (recommended: less than 50 characters)
2. Written in sentence case (starts with a capital letter)
    - Good: <span class="good">Add information about wheels</span>
    - Bad: <span class="bad">Add Information About Wheels</span>
3. Written in the imperative (like a command), not the past tense
    - Good: <span class="good">Fix installation of NavX page</span>
    - Bad: <span class="bad">Fixed installation page</span>
