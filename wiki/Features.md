# Features

The tabs along the top are **Single**, **Batch**, **Instagram**, **Watermark**, **Tracker** and **Schedule**, with **Options** on the right.

## Scrub

Strips GPS location, device details, dates, encoder tags and edit history from your videos. Nothing is re-encoded, so there's no quality loss.

- **Single**: one video at a time.
- **Batch**: many videos at once.
- **Options**: controls exactly what gets scrubbed. The same settings are used when other features scrub for you (for example "Scrub after watermarking").

## Watermark

Puts your logo on every video, so reposts still show where they came from.

1. Open **Watermark** and click **Change logo** (or drop an image on the page).
2. Pick one of nine **positions**, and set **Size**, **Opacity** and **Margin**. The preview updates live.
3. Add videos (**Choose videos** or drag them in) and pick a **Save to** folder.
4. Leave **Scrub after watermarking** on to strip metadata at the same time.
5. Click **Watermark all**.

## Schedule

Upload and schedule Shorts to the YouTube channels you own.

- **Connect a channel** to sign in with Google. Connect as many channels as you like.
- **Add videos** to a channel, or give it an **Inbox folder** so videos dropped there are picked up.
- **Spread videos across channels** shares a batch out, one channel per video.
- **Calendar & settings** on each channel opens:
  - **Weekly calendar**: design the times you post each week. The Recommendations panel flags problems such as posts too close together or not enough queued videos.
  - **Next 7 days**: what's coming up.
  - **Post settings**: made for kids, AI-content disclosure, tags, hashtags on every post, text added to every description, **Style notes for the AI**, category, language, license, and options like **Approve titles before upload** and **Pause this channel**. Use **Save as default** or **Apply to all channels** to reuse them.
- The **Queue** shows every video, its channel, title, hashtags, post time and status. Videos marked **Needs review** wait until you click **Approve** (or **Edit**).
- The top right shows today's **YouTube quota** use (YouTube allows 10,000 units a day) and roughly how many more uploads fit.
- Removing a channel lets you move its waiting videos to your other channels.

## AI titles

MetaScrub writes a title, description and hashtags for each video you schedule. It looks at **four still frames** from the video, plus its file name and that channel's **Style notes for the AI**, and learns from your best-performing Shorts.

This needs your own AI API key, added in **Schedule → Settings** (OpenRouter or Anthropic). To set it up with OpenRouter and choose a model, see **[OpenRouter: API Key and Choosing a Model](OpenRouter-Setup)**. Without a key, nothing is sent to an AI service and titles are made from the file name instead.

A tag limit counter warns you before you go over YouTube's tag limit.

## Tracker

Live stats for your channels: 24-hour and longer gains, how fast your newest Short is moving compared with usual, and which hashtags work best. Turn on **Live** to refresh every minute. The Tracker reads public statistics using your own YouTube API key.

## Discord alerts

Get a message in your Discord server when:

- **A video is uploaded**: when it's scheduled on YouTube, and again when it goes live.
- **Something needs you**: an upload failed, a channel signed out, or the daily quota ran out.
- **A Short is going viral**: a recent Short is far ahead of your usual pace (for example 3× your usual views and at least 1,000 views). You get another message each time its views double. This needs the channel in the Tracker tab.

To set it up:

1. In Discord, open your server's **Server Settings → Integrations → Webhooks**.
2. Click **New Webhook**, pick the channel for alerts, then **Copy Webhook URL**.
3. Paste it into MetaScrub's **Discord alerts** window, choose which alerts you want, and click **Send test message**.
4. Click **Save**.

## Update check

MetaScrub checks for new versions and tells you when one is available. Download it from the [releases page](https://github.com/MikeytScripts/MetaScruber/releases/latest).
