slack-to-discord-timeshift
==========================

This tool takes a Slack export file and imports it into a Discord server, on a timeshifted basis.

Differences between this and the original (https://github.com/pR0Ps/slack-to-discord):

* Puts everything into a single channel, with a `\[#channelname]` prefix and a "$user in $year" username.
* Doesn't fake avatars
* Doesn't change topic or pin messages
* Starts from $now - $timeshift, and only posts messages and actions when they are roughly $timeshift ago.


# To run:

```
$ slack-to-discord --zipfile <slack export zip> --guild <server name> --token <bot token> --timeshift <timeshift in days> --destchannel <destchannel>
```

