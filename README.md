# Thing — Where Humans Meet
This is a first attempt at building an image for a generic video conferencing solution supporting multiple video conferencing systems. It is based upon the template [ublue-os/image-template](https://github.com/ublue-os/image-template).

# Goal
Several commercial video conferencing providers offer certified hardware to integrate into their video conferencing solutions. For Free video conferencing solutions it is unfeasible to offer similarly certified and integrable solutions. But an image that allows to simplify setup of off-the-shelf for use with Free video conferencing systems seems like a realistic goal

# Roadmap
Current state (as of last update of this README.md) is image builds but nothing is functional.

First step is to get it up and running, boot into a First Boot mode and query some connection parameters. The whole UX is still work-in-progress.

The idea is to allow use of different Free video conferencing systems. As we want to use Nextcloud Talk, that's the one we start with.

Then, there's Jitsi as an easily available solution which could be supported.

Big Blue Button is also in use at our place, so that one's also on the menu.

OpenTalk would be nice to support, but we don't have access to an instance, yet.

Of course, the video conferencing market is heavily fragmented. Even with Free video conferencing systems in our focus we still see the necessity to offer access to proprietary video conferencing systems. Those might not be as integrated as they might be with the hardware offered by their respective vendors and their partners, though.

# Design
SteamOS and Bazzite are my role models in this regard. But instead of booting into Gamingmode, Thing should boot into an "upcoming events" screen (after initial setup of course) offering to join an event or start a video conference.

Thing should allow being controlled by either a simple remote control with d-pad and two buttons for confirmation and back navigation.

Thing should allow being controlled by a secondary display with touchscreen.

Thing should serve a web UI to control it remotely.

Thing should allow switching to a desktop mode where other video conferencing solutions can be accessed using a browser or an application from Flathub.

Thing should be immutable. Changes to its configuration besides connection to its primary video conferencing systems should not survive reboots.

Updates should be robust and revertible.