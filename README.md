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
