# University of Alberta DemoStudent block plugin for Moodle

## What does it do?

The DemoStudent block gives instructors a way to enroll a
"demostudent" in their course, then switch back and forth between
their instructor view and the student view.

## What is all this code?

This repository contains a copy of Moodle 2.4, along with the
DemoStudent block plugin.  The plugin itself is contained entirely
within the blocks/demostudent/ directory.

## Caveats

When the plugin is installed through the Moodle Notifications page, it
will create a role named 'demostudent' if one does not already exist.
If your system already has such a role, the plugin may not function as
expected.

## Tested with

Moodle 2.4.5
Moodle 2.4.7

## Repositories

Moodle core + plugin:
https://github.com/ualberta-eclass/moodle-block_demostudent

Plugin only:
https://moodle.org/plugins/view.php?plugin=block_demostudent

## Installation

### Method 1 - tarball

1. Download and untar from moodle plugin site:
https://moodle.org/plugins/view.php?plugin=block_demostudent
2. Copy blocks/demostudent/ folder into your moodleinstall/blocks/.
3. On your Moodle site, browse to:
My home / Site administration / Notifications
4. Install the new plugin.

### Method 2 - git integration

Use if your moodle installation is under git control.

1. Add github repository as new remote:
git remote add demostudent git://github.com/ualberta-eclass/moodle-block_demostudent.git
2. git fetch
3. checkout your deployment branch.
4. merge from the Moodle version branch matching your development branch base.  eg. git merge contextadmin_24_STABLE
5. Install the new plugin from the Moodle admin Notification page as above.
