# [matrix-commander-gael](https://snapcraft.io/matrix-commander-gael)


_This is NOT an original piece of work, just a snap of matrix-commander_

This program is a simple but convenient app to send and receive Matrix messages from the CLI in various different ways.
Use cases for this program could be
* a bot or part of a bot,
* to send alerts,
* combine it with cron to publish periodic data,
* send yourself daily/weekly reminders via a cron job
* send yourself a daily song from your music collection
* a trivial way to fire off some instant messages from the command line
* to automate sending via programs and scripts
* a "blogger" who frequently sends messages and images to the same room(s) could use it
* a person could write a diary or run a gratitutde journal by sending messages to her/his own room
* as educational material that showcases the use of the matrix-nio SDK

**Create an alias for ease of use (optional)**

`sudo snap alias matrix-commander-gael.matrix-commander matrix-commander`

**First-time users**

Read https://github.com/8go/matrix-commander#examples-of-calling-matrix-commander

**2025-06-30**
* New build to resolve CVE-2025-50181/USN-7599-2

**2025-06-20**
* New build to resolve CVE-2025-4517/CVE-2025-4435/CVE-2025-4330/CVE-2025-4138/CVE-2024-12718/USN-7583-1

**2025-06-17**
* New build to resolve CVE-2025-1795/CVE-2025-4516/USN-7570-1

**2025-03-12**
* New build to resolve CVE-2024-9287/CVE-2024-12254/CVE-2025-0938/USN-7116-1/USN-7219-1/USN-7280-1

**2024-11-01**
* Improvements, up to v8.0.0
* Added minor changes to allow sending files/images to unverified rooms
* Changed --get-room-info does no longer return "creator"

**2024-09-17**
* New build to resolve CVE-2024-6923/CVE-2024-6232/CVE-2024-8088/CVE-2023-27043/CVE-2024-7592/USN-7015-1

**2024-09-14**
* New build to resolve CVE-2024-6345/USN-7002-1

**2024-09-04**
* Improvements, up to v7.7.0
* Added new feature: --verify manual does a one-way setting of trust
* Added new feature: --verify emojireq initiates an emoji verification (instead of waiting for one)

**2024-08-03**
* New build to resolve CVE-2024-4032/USN-6941-1

**2024-05-08**
* Improvements, up to v7.6.2

* Using core24 to update the Python runtime
* Targeting Python v3.12 following https://github.com/8go/matrix-commander/issues/168


**2024-03-31**

* Improvements, up to v7.6.0

* Added feature "time" to --download-media-name
* Added new feature: --room-dm-create-allow-duplicates
* Added new feature: --joined-dm-rooms to list all joined DM rooms of current user

**2023-10-11**

* Improvements, up to v7.3.1

* New feature --download-media-name SOURCE|CLEAN|EVENTID

**2023-09-13**

* New build to resolve CVE-2022-48554/USN-6359-1

**2023-06-06**

* Improvements, up to v7.2.0

* Enhancement: feature --room-invites is now also available without --listen

* New build to resolve CVE-2023-24329/USN-6139-1

**2023-04-19**

* Improvements, up to v7.1.0

* New feature --room-invites LIST|JOIN|LIST+JOIN

**2023-04-12**

* Improvements, up to v7.0.0

* Support for emojize

**2023-04-04**

* Improvements, up to v6.0.2

* Fix for error when providing wrong password at login

**2023-03-18**

* New build to resolve CVE-2023-24329/USN-5960-1
* Dependencies cleanup

**2023-03-17**

* New build to resolve CVE-2023-24329/USN-5960-1

**2023-03-01**

* New build to resolve CVE-2022-40898/USN-5821-3

**2023-01-24**

* New build to resolve CVE-2022-40897/USN-5817-1

**2022-12-28**

* New build to switch to core22 as most of the users are on Ubuntu 22.04

* Improvements, up to v6.0.1

* Fix for opening web browser for SSO

**2022-12-09**

* New build to resolve CVE-2022-37454/CVE-2022-45061/USN-5767-1

**2022-11-23**

* Improvements, up to v5.0.0

* Added --sync off|full to allow turning sync off for send actions, default is --sync full
* Bug fix in --joined-members, added initial part of new feature --output
* -output is currently only implemented for 2 functions: --joined-members and --joined-rooms
* Added new option --get-room-info to get room alias, room display name, and much more
* Improved --room-get-info to allow also aliases instead of room id
* Added new option `--get-client-info`
* Added new type `json-spec` to `--output`
* Added new option `--verbose`
* Changes to --output, `json-spec` only provides output for `--listen`
* Added --output format logic also to --version
* 2 bug fixes: --room-create failed for empty aliasm --joined-members failed when avatar missing
* New feature: --plain now available for --room-create and --room-dm-create
* Improved error logging

**2022-10-03**

* Improvements, up to v3.5.1

* Minor bug fix for --tail

**2022-08-02**

* Improvements, up to v3.5.0

* Added room alias to room id conversion for sending images
* Minor modifications to handle SVG files better as images
* Minor fix for sending SVG files
* Added feature "--logout" to logout and remove device from use
* Allow all actions to be performed in the same command
* Added "--login", re-did internals to allow more parallelism
* New features "--room-resolve-alias" and "--room-set-alias"
* Added new feature "--room-set-alias" to add an alias to a room
* Added new feature "--room-get-state" to print state of room(s)
* Added new feature "--room-get-visibility" to find out if room is private or public
* New option "--has-permission"
* Added feature "--get-profile" to print user profile(s)
* Added feature "--print-event-id" also to sending actions

**2022-07-15**

* New build to resolve CVE-2015-20107/USN-5519-1

**2022-06-11**

* Improvements, up to git commit ecc78d7 (2022-06-10)

* Only reads from keyboard if there are no other actions
* Added DM (Direct Messaging) feature
* Added option "--whoami"
* Added feature "--get-display-name"
* Added features --set-presence and --get-presence
* New features: --download and --upload and --separator
* Added feature --mxc-to-http
* New features: --devices, --discovery-info, --login-info
* Added features: --upload, --download, --delete-mxc, --file-name, --key-dict, --access-token
* Added feature --rest to invoke the Matrix REST API
* Added feature --delete-mxc-before
* Added features --set-avatar and --get-avatar
* Added features --export-keys and --import-keys
* Added feature --get-openid-token
* Added feature --delete-device to delete devices
* Added feature --room-redact to delete messages, images, files, etc. from client GUIs

**2022-05-29**

* Improvements, up to git commit 08e5859 (2022-05-26)

* Bug fix in --event code
* Introduced an event-templates "repository"

**2022-05-24**

* Many improvements, up to git commit d10ce45 (2022-05-23)

* Made matrix-commander.py executable
* Add SSO support using browser to complete login
* Add command to set display-name for authenticated user
* Correct exit status
* Prefix additional lines in multiline messages with space
* Updated from asyncio.get_event_loop().run_until_complete to asyncio.run
* Allow to disable SSL certificate validation
* Exit gracefully when store or credentials are missing
* Added the new commandline options like --no-ssl and --display-name
* Added pipe and stdin management to images
* Added new feature --ssl-certificate
* Added option --no-sso
* Added "-" for piped stdin input to audio and files as well
* Added --event to send arbitrary Matrix events
* Bug fixes in --ssl-certificate code

**2022-03-29**

* New build to resolve CVE-2022-0391/USN-5342-1

**2021-12-18**

* New build to resolve CVE-2021-3737/USN-5201-1

**2021-10-18**

* First version of this snap based on matrix-commander 2021-07-23
