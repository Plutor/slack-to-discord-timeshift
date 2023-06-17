slack-to-discord-timeshift
==========================

This tool takes a Slack export file and imports it into a Discord server, on a timeshifted basis.

Differences between this and the original (https://github.com/pR0Ps/slack-to-discord):

* Puts everything into a single channel, with a \[#channelname] prefix.
* Starts from $now - $timeshift, and only posts messages and actions when they are roughly $timeshift ago.

