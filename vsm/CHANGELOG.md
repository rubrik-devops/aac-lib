# aac-lib
AAC Library of Tools

- <a href=https://github.com/Texiwill/aac-lib/tree/master/>List of Tools</a>

## vsm
Linux Version of VMware Software Manager

### Support
Email elh at astroarch dot com for assistance or if you want to add
for more items.

### Data file Changelog
- 1.0.35 - Updates for 6.0 DriversTools, 6.5U2 CustomIso
- 1.0.34 - Updates to VR81
- 1.0.33 - Updates for 6.7 DriversTools
- 1.0.32 - Updates for 6.5U2 DriversTools
- 1.0.31 - Updates for DriversTools & 4.6.2 compatibility
- 1.0.30 - Updates for 6.0 DriversTools
- 1.0.29 - 4.6.1 compatibility
- 1.0.28 - Updates for 6.7 and other DriversTools
- 1.0.27 - Updates for 6.7 DriversTools
- 1.0.26 - 4.6.0 compatibility
- 1.0.25 - More DriversTools updates w/duplicate deletions that caused issues
- 1.0.24 - More DriversTools updates
- 1.0.23 - Fix for DriversTools
- 1.0.22 - ESXI65U2 Updates
- 1.0.21 - 4.5.9 compatibility
- 1.0.20 - 4.5.8 compatibility
- 1.0.19 - latest updates and 4.5.7 compatibility
- 1.0.18 - latest updates and 4.5.6 compatibility
- 1.0.17 - vSphere DriversTools Updates, VMware Tools Updates
- 1.0.16 - ovftool duplicates
- 1.0.15 - vSphere DriversTools Updates
- 1.0.14 - latest updates and 4.5.5 compatibility
- 1.0.13 - Updates for VR81
- 1.0.12 - Several smaller updates for 6.5, Converter, etc.
- 1.0.11 - VR81 Update
- 1.0.9 - vSphere 6.7
- 1.0.8 - New Drivers
- 1.0.7 - Keep up with 4.5.3
- 1.0.6 - Keep up with 4.5.2
- 1.0.5 - Updates for 6.5/6.0 new drivers
- 1.0.4 - Updates for vRealize Updates
- 1.0.3 - Updates for 6.0 new drivers
- 1.0.2 - Updates for 6.0 new drivers
- 1.0.1 - added support for new packages and fixed missing files
- 1.0.0 - Initial Release

### Changelog
4.6.3 - Small Debug fix

4.6.2 - Fixed a small bug in display

4.6.1 - Fixed --fav bug with parsing

4.6.0 - Download logic bug fixed for differently formated HTML

4.5.9 - Menu logic bug fixed

4.5.8 - Infrastructure Operations Management added back to top

4.5.7 - Small changes for new options

4.5.6 - Update for new Windows VSM Data Files and new options

4.5.5 - Update to install.sh to create the update.sh automatically

4.5.5 - added --fav option to allow for using favorites from commandline
        (no more need to Mark a Favorite)

4.5.4 - Fixed some logic for download paths

4.5.3 - Fixed several bugs: Malformed Data causing download error
        (@ivirtualex),--dlg with older packages, error messages in wrong spot, 
	inappropriate data file errors, code cleanup, and added to logic for 
	download paths.

4.5.2 - Fixed logic for download paths, logic for showing checksum
        failures

4.5.1 - Fixed --dlg error and added some missing data. Datafile 1.0.1 now
        Special thanks to Alex Lopez (@ivirtualex) and 
	Mike Laverick (@m_laverick)

4.5.0 - Rewrite to better allow updates, --dlg to work, sha256/sha1 sums, and improved MacOS support, not to mention improvements in performance

4.0.4 - MacOS Support

4.0.3 - Small Bug with --dlg fixed, plus initial download speedup

4.0.2 - Support for VC55U3H, 60U3 fixes, and --dlg updates thanks to Michelle Laverick (@m_laverick)

4.0.1 - Support for VC65U1G plus bugfix from Alex Lopez (@ivirtualex)

4.0.0 - My VMware now default, cleaned up Debug more

3.9.0 - Added Debian Support

3.8.1 - Hopefully the last progress issue

3.8.0 - One more progress issue.

3.7.9 - Bug fix in progress. My thanks to Alex Lopez (@ivirtualex) for finding.

3.7.8 - Bug fix when missing .vsmrc, fixes to progress. My thanks to Alex
Lopez (@ivirtualex) for finding the bug.

3.7.7 - slight change to versioning of a package

3.7.6 - Changes to how .vsmrc is processed to support Docker. .vsmrc can 
now be in $HOME, Repo Dir, or VSM XML Dir (/tmp/vsm). If the .vsmrc is
in any directory besides the default or $HOME you will need to specify
the --repo or -v|--vsmdir options and order is important.

3.7.5 - Fix to progress bars once more, should be final form. Added another
suite and fixed more broken due to new version downloads.

3.7.4 - Fixed missing progress when -nq specified

3.7.3 - Improved progress to include download progress

3.7.2 - Minor bug fix to allow proper download of VRNI

3.7.1 - Minor bug fix when encountering My VMware package that contains
VSM packages, added quiet and progress flags, and a slight code reorganization.

3.7.0 - CustomIso (OEM), and DriverTools can now be downloaded for all
My VMware packages where they exist.

3.6.0 - -mr now implies -m, added Mark capability to -m, fixed wget not
	using cookies all the time

3.5.5 - Fixed download of VVD issue 

3.5.4 - Fixed download directory issue

3.5.3 - More option issues corrected.

3.5.2 - Fixed some downloads (VRLI for vCenter and others) thanks to fellow 
	vExperts Michael Rudluff and Rotem Agmon

3.5.1 - Missing option corrected

3.5.0 - Using My VMware to pick up the up to date names instead of hardcoding 
	them. Added VMware Validated Design (VVD). Fixed VRNI and AppVolumes. 
	Also added the need for jq rpm, a JSON interpreter, for the 
	up-to-date names.

3.2.4 - Protection for temporary directory were reversed

3.2.3 - Protections from temporary directory owned by wrong user causing
	connection errors

3.2.2 - Protections from running as root and added install.sh to repo

3.2.1 - Minor fix... Fusion wrong file uploaded!

3.2.0 - Added Support for VMware Fusion download and improved errors when
	there are network issues.

3.1.0 - Added support for VMware Horizon, VMware Horizon Clients, and VMware 
	Workstation Pro. For now the Fusion download is within VMware Horizon.

3.0.1 - fixed a grep error showing up when it should not

3.0.0 - -m|--myvmware option now works including the need to install the 'bc'
	package. You can now download packages from My VMware not just view 
	missing packages!  Some things may still need tweaking, however. Also,
	added the -mr option to reset My VMware information only.  Email 
	issues and output using the --debug flag to elh at astroarch dot com.

2.5.2 - Fix to --dlg for single file downloads. Local was missing

2.5.1 - Protection for wildcard option

2.5.0 - Code reorganization and addition of wildcard option

2.0.2 - Fixed bug with single file selection

2.0.1 - Fixed bug where you were able to mark missing suites

2.0.0 - Added ability to get missing suite information from VMware's website
        Fixed the ability to select menu options using wrong input

1.7.0 - Fixed an intialization problem. Required --reset|-r to initialize

1.6.9 - Fixed issue where download was not happening for All when
individual files are listed.

1.6.8 - Fixed issue where individual file download resulted in bad
menu display

1.6.7 - Prompts for creds specific My VMware now

1.6.6 - fixed single file download and readme

1.6.5 - added --nooem|--oem, --nodts|--dts, --nooss|--oss to the .vsmrc
configuration file when options are saved

1.6.1 - moved variable and removed check for perl-XML-XPath as it is no
longer required.

1.6.0 - cleaned up code pulling unique items into one loop not 3
separate loops. Fixed Mark to only appear in one spot.

1.5.0 - added ability to download specific file by name or part of a
name and fixed major bug on associated products list where resultant
list was malformed

1.1.0 - fixed 'Back' to actually send you back just 1 level at all times
by creating a path variable that gets updated for every menu call and
Back used

1.0.1 - fixed 'Back' menu item when actual packages are shown

1.0.0 - added Minimum_Required menu item, do only download the base files
and not OpenSource, DriversTools, or CustomIso. Also added the
--dts|--nodts, --oem|--nooem, --oss|--nooss to set what to download when
any of the 'All' styles are selected.

0.9.5 - fixed latest parsing. It was too broad and did not confine to
the latest of a specific major version. I.e. 60 vs 65

0.9.4 - fixed issue where too much was include in the 'smarts'. Main
Product Downloads were being placed into CustomIso and DriverTools.

0.9.3 - Initial public launch
