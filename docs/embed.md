# Commands: Embed

## Using CLYPPY to Embed Videos in Discord

CLYPPY can help you share videos from multiple platforms in your Discord chats. Simply call the `/embed` command with the link to the supported video, and CLYPPY will do the rest of the work.

See [Supported Video Types](#supported-video-types) to view a list of all video platforms that CLYPPY can embed.

```{admonition} Usage
:class: tip
`/embed url=[Video link]`
```

![](images/tiktok-embed.gif)

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

| Video Platform | Supported                                                  | Notes                              |
|----------------|------------------------------------------------------------|------------------------------------|
| twitch.tv      | <span style="color:green;font-size:1.5em;">&#10004;</span> | Also adds Twitch Chat to the embed |
| youtube.com    | <span style="color:green;font-size:1.5em;">&#10004;</span> | Supports videos under 5 minutes    |
| tiktok.com     | <span style="color:green;font-size:1.5em;">&#10004;</span> | Supports most tiktok links         |
| vimeo.com      | <span style="color:red;font-size:1.5em;">&#10007;</span>   | Planned to be added                |
