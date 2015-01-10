OpenMW: A reimplementation of The Elder Scrolls III: Morrowind
==============================================================

[![Build Status](https://travis-ci.org/OpenMW/openmw.svg?branch=coverity_scan)](https://travis-ci.org/OpenMW/openmw)

[![Coverity Scan Build Status](https://scan.coverity.com/projects/3740/badge.svg)](https://scan.coverity.com/projects/3740)

OpenMW is an attempt at recreating the engine for the popular role-playing game
Morrowind by Bethesda Softworks. You need to own and install the original game for OpenMW to work.

* Version: 0.34.0
* License: GPL (see docs/license/GPL3.txt for more information)
* Website: http://www.openmw.org
* IRC: #openmw on irc.freenode.net

Font Licenses:
* DejaVuLGCSansMono.ttf: custom (see docs/license/DejaVu Font License.txt for more information)

Getting Started
===============

* [Official forums](https://forum.openmw.org/)
* [Installation instructions](https://wiki.openmw.org/index.php?title=Installation_Instructions)
* [Build from source](https://wiki.openmw.org/index.php?title=Development_Environment_Setup)
* [Testing the game](https://wiki.openmw.org/index.php?title=Testing)
* [How to contribute](https://wiki.openmw.org/index.php?title=Contribution_Wanted)
* [Report a bug](http://bugs.openmw.org/projects/openmw) - read the [guidelines](before submitting your first bug!)
* [Known issues] (http://bugs.openmw.org/projects/openmw/issues?utf8=%E2%9C%93&set_filter=1&f%5B%5D=status_id&op%5Bstatus_id%5D=%3D&v%5Bstatus_id%5D%5B%5D=7&f%5B%5D=tracker_id&op%5Btracker_id%5D=%3D&v%5Btracker_id%5D%5B%5D=1&f%5B%5D=&c%5B%5D=project&c%5B%5D=tracker&c%5B%5D=status&c%5B%5D=priority&c%5B%5D=subject&c%5B%5D=assigned_to&c%5B%5D=updated_on&group_by=tracker)

The data path
=============

The data path tells OpenMW where to find your Morrowind files. If you run the launcher, OpenMW should be able to pick up the location of these files on its own, if both Morrowind and OpenMW are installed properly (installing Morrowind under WINE is considered a proper install).

Command line options
====================

<pre>
Syntax: openmw <options>
Allowed options:
  --help                                print help message
  --version                             print version information and quit
  --data arg (=data)                    set data directories (later directories
                                        have higher priority)
  --data-local arg                      set local data directory (highest
                                        priority)
  --fallback-archive arg (=fallback-archive)
                                        set fallback BSA archives (later
                                        archives have higher priority)
  --resources arg (=resources)          set resources directory
  --start arg (=Beshara)                set initial cell
  --content arg                         content file(s): esm/esp, or
                                        omwgame/omwaddon
  --anim-verbose [=arg(=1)] (=0)        output animation indices files
  --no-sound [=arg(=1)] (=0)            disable all sounds
  --script-verbose [=arg(=1)] (=0)      verbose script output
  --script-all [=arg(=1)] (=0)          compile all scripts (excluding dialogue
                                        scripts) at startup
  --script-console [=arg(=1)] (=0)      enable console-only script
                                        functionality
  --script-run arg                      select a file containing a list of
                                        console commands that is executed on
                                        startup
   --script-warn [=arg(=1)] (=1)        handling of warnings when compiling
                                        scripts
                                        0 - ignore warning
                                        1 - show warning but consider script as
                                        correctly compiled anyway
                                        2 - treat warnings as errors
  --skip-menu [=arg(=1)] (=0)           skip main menu on game startup
  --new-game [=arg(=1)] (=0)            run new game sequence (ignored if
                                        skip-menu=0)
  --fs-strict [=arg(=1)] (=0)           strict file system handling (no case
                                        folding)
  --encoding arg (=win1252)             Character encoding used in OpenMW game
                                        messages:

                                        win1250 - Central and Eastern European
                                        such as Polish, Czech, Slovak,
                                        Hungarian, Slovene, Bosnian, Croatian,
                                        Serbian (Latin script), Romanian and
                                        Albanian languages

                                        win1251 - Cyrillic alphabet such as
                                        Russian, Bulgarian, Serbian Cyrillic
                                        and other languages

                                        win1252 - Western European (Latin)
                                        alphabet, used by default
  --fallback arg                        fallback values
  --no-grab                             Don't grab mouse cursor
  --activate-dist arg (=-1)             activation distance override
</pre>

Changelog
=========

See CHANGELOG.md
