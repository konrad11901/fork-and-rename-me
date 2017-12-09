<h1 align="center">tosheets</h1>
<p align="center"><b>This is the snap for tosheets</b>, <i>"A simple command line utility that sends your stdin to sheets"</i>. It works on Ubuntu, Fedora, Debian, and other major Linux
distributions.</p>

[![Snap Status](https://build.snapcraft.io/badge/konrad11901/tosheets-snap.svg)](https://build.snapcraft.io/user/konrad11901/tosheets-snap)

> The author of this tool is **kren1**. The original repository can be found [here](https://github.com/kren1/tosheets).
<!-- Uncomment and modify this when you are provided a build status badge
<p align="center">
<a href="https://build.snapcraft.io/user/snapcrafters/fork-and-rename-me"><img src="https://build.snapcraft.io/badge/snapcrafters/fork-and-rename-me.svg" alt="Snap Status"></a>
</p>
-->

## Install

    sudo snap install tosheets

([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

## How to use it
    $ tosheets -h
    tosheets, send stdin to your google sheets

    Usage:
      tosheets -c <cell> [-u] [-s <sheet>] [--spreadsheet=<spreadsheet>] [--new-sheet=<name>] [-d <delimiter>]
      tosheets (-h | --help)
      tosheets --version
      
    Options:
      -h --help                     Prints help.
      --version                     Show version.
      -u                            Update CELL(s) instead of appending.
      -c CELL                       Start appending to CELL.
      -s SHEET                      Use sheet name SHEET, otherwise tries to use TOSHEETS_SHEET (default: first visible sheet). 
      -d DELIMITER                  Use DELIMITER to split each line (default: whitespace).
      --spreadsheet=<spreadsheet>   Send to the spreadsheet identified by spreadshetId (ie. docs.google.com/spreadsheets/d/<spreadsheetId>/...), if empty uses TOSHEETS_SPREADSHEET enviroment variable.                                
      --new-sheet=<name>            Create a new spreadsheet with the chosen name. Prints the spreadsheetId so it can be piped/stored.


## Known issues

* ~When running tosheets for the first time, it should open the default browser with the Google Account login page loaded. Unluckily, it doesn't work, so you need to open the outputted link manually. This issue doesn't occure if the snap is installed in devmode.~ This bug has been fixed (see [here](https://github.com/konrad11901/tosheets-snap/pull/1)).

<p align="center">Published for <img src="http://anything.codes/slack-emoji-for-techies/emoji/tux.png" align="top" width="24" /> with :gift_heart: by Snapcrafters</p>

## Remaining tasks

Snapcrafters ([join us](https://forum.snapcraft.io/t/join-snapcrafters/1325)) 
are working to land snap install documentation and
the [snapcraft.yaml](https://github.com/snapcrafters/fork-and-rename-me/blob/master/snap/snapcraft.yaml)
upstream so [Project] can authoritatively publish future releases.

  - [x] Fork the [Snapcrafters template](https://github.com/snapcrafters/fork-and-rename-me) repository to your own GitHub account.
  - [x] Rename the forked Snapcrafters template repository
  - [x] Update logos and references to `[Project]` and `[my-snap-name]`
  - [x] Create a snap that runs in `devmode`
  - [x] Register the snap in the store, **using the preferred upstream name**
  - [ ] Add a screenshot to this `README.md` _is it neccessary in this case?_
  - [x] Publish the `devmode` snap in the Snap store edge channel
  - [x] Add install instructions to this `README.md`
  - [x] Update snap store metadata, icons and screenshots
  - [x] Convert the snap to `strict` confinement, or `classic` confinement if it qualifies
  - [x] Publish the confined snap in the Snap store beta channel
  - [x] Update the install instructions in this `README.md`
  - [x] Post a call for testing on the [Snapcraft Forum](https://forum.snapcraft.io) - [link](https://forum.snapcraft.io/t/call-for-testing-tosheets/3109/1)
  - [x] Ask a [Snapcrafters admin](https://github.com/orgs/snapcrafters/people?query=%20role%3Aowner) to fork your repo into github.com/snapcrafters, transfer the snap name from you to snapcrafters, and configure the repo for automatic publishing into edge on commit _(asked via Code-in dashboard)_
  - [x] Add the provided Snapcraft build badge to this `README.md`
  - [x] Publish the snap in the Snap store stable channel
  - [x] Update the install instructions in this `README.md`
  - [ ] Post an announcement in the [Snapcraft Forum](https://forum.snapcraft.io) - [link]()
  - [ ] Submit a pull request or patch upstream that adds snap install documentation - [link]()
  - [ ] Submit a pull request or patch upstream that adds the `snapcraft.yaml` and any required assets/launchers - [link]()
  - [ ] Add upstream contact information to the `README.md`  
  - If upstream accept the PR:
    - [ ] Request upstream create a Snap store account
    - [ ] Contact the Snap Advocacy team to request the snap be transferred to upstream
  - [ ] Ask the Snap Advocacy team to celebrate the snap - [link]()

If you have any questions, [post in the Snapcraft forum](https://forum.snapcraft.io).

<!-- 
## The Snapcrafters

| [![Your Name](http://gravatar.com/avatar/bc0bced65e963eb5c3a16cab8b004431/?s=128)](https://github.com/yourname/) |
| :---: |
| [Your Name](https://github.com/yourname/) |
--> 

<!-- Uncomment and modify this when you have upstream contacts
## Upstream

| [![Upstream Name](http://gravatar.com/avatar/bc0bced65e963eb5c3a16cab8b004431?s=128)](https://github.com/upstreamname) |
| :---: |
| [Upstream Name](https://github.com/upstreamname) |
-->
