# Commands: Log

## User Chat Logging for twitch.tv

As a social integration bot, CLYPPY has multiple features for working with Twitch, one of them being the `/log` command.

The `/log` command is used for retrieving all messages sent in the Twitch Chat of the specified Twitch Channel, sent by a specific Twitch User. 

```{admonition} Usage
:class: tip
`/log user=[Twitch user] channel=[Twitch channel]`
```

Both `user` and `channel` must be a Twitch username, like `xqc`, `kyedae`, etc.

---

## Optional Parameters

The `/log` command also has two optional params, `month` and `year`.

If you want to specify a specific time to retrieve chatlogs from, you can use these parameters. 

- `year` must be just the year number, for example `2021`.
- `month` must be the month number - for example January would be `1`, July would be `7`, and so forth.

```{note}
If you choose to use any of the optional parameters, you must give a specific value for both `year` and `month`. Giving only `month` and leaving `year` blank, or vice versa, will not work.
```