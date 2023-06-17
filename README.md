slack-to-discord-timeshift
==========================

This tool takes a Slack export file and imports it into a Discord server, on a timeshifted basis.

Differences between this and the original (https://github.com/pR0Ps/slack-to-discord):

* Doesn't fake usernames or avatars
* Puts everything into a single channel, with a `\[#channelname] <username>` prefix.
* Starts from $now - $timeshift, and only posts messages and actions when they are roughly $timeshift ago.


# To run:

```
$ slack-to-discord --zipfile <slack export zip> --guild <server name> --token <bot token> --timeshift <timeshift in days> --ddestchannel <destchannel>
```

