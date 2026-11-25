# Privacy Notice

## Information handled by the application

The application reads CAN-bus messages locally through the PCAN interface and displays them in the application. The source code reviewed for this notice does not send CAN-bus messages, the local hardware identifier, or the local licence key to the update service.

## Update checks and downloads

After startup, the application automatically requests its configured version manifest from GitHub to check whether an update is available. If the user chooses to install an offered update, the application downloads the release archive from the URL in that manifest. GitHub receives the ordinary network request information needed to serve these requests, such as the requesting IP address and request metadata. The update check can be avoided by preventing the application from accessing the network; there is currently no in-app setting to disable it.

The configured manifest and release URL are maintained by the project. Users should download releases only from the project's linked GitHub release page and verify the published checksum and signature information.

## Local data

The application stores its licence key in a file in the current Windows user's home directory. It also writes update files to a local staging directory while applying an update. These files are not sent to GitHub by the code path described above.

## Changes to this notice

This notice should be reviewed whenever update, licensing, or network behavior changes.
