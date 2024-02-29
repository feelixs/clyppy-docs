# Commands: Embed

## Using CLYPPY to Embed Videos in Discord

CLYPPY can help you share videos from multiple platforms in your Discord chats. Simply call the `/embed` command with the link to the supported video, and CLYPPY will do the rest of the work.

See {ref}`supported-video-types` to view a list of all video platforms that CLYPPY can embed.

```{admonition} Usage
:class: tip
`/embed url=[Video link]`
```

It may take some time for the video to be processed by CLYPPY before you see it embedded into your chat. 

If other users have submitted embed requests before you, your embed will be but into a queue behind them.

```{note}
You can only have one embed request in the queue at once. After submitting a request by using the `/embed` command, you'll need to wait until after that request has been finished processing before using `/embed` again.
```

## Optional Parameters

The `/embed` commands also has two optional parameters, `with_chat` and `enable_preview`.

- `with_chat`: for Twitch Clip embeds, set this to `True` to show the Twitch Chat inside the Video Embed.
- `enable_preview`: By default, CLYPPY will automatically downscale videos to be uploadable to Discord. If you set `enable_preview` to `False`, though, CLYPPY will not downscale and, if it's too large for Discord, will direct you to download the fetched video file (without embedding it to Discord).

## Supported Video Types:

| Video Platform | Supported                                           |
|----------------|-----------------------------------------------------|
| twitch.tv      | <style>span[class="checked"]{color: green;}</style> |
| youtube.com    | <style>span[class="checked"]{color: green;}</style> |
