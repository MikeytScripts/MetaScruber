# FAQ and Troubleshooting

**Windows says "Windows protected your PC".**
The app isn't code-signed yet. Click **More info → Run anyway**.

**Which download do I need?**
`MetaScrub.exe` for almost every PC. `MetaScrub-arm64.exe` only for Windows on ARM laptops. See [Getting Started](Getting-Started#1-download).

**Can I use my license key on two PCs?**
No. Each key activates on one PC. Ask on [Discord](https://discord.gg/HnqkyDkFUA) if you've changed computers.

**Does scrubbing lower the quality?**
No. Nothing is re-encoded.

**AI titles aren't being written.**
- Check that your API key is entered and still exists on [openrouter.ai/keys](https://openrouter.ai/keys).
- Check you have credits, or that the key's credit limit isn't used up.
- Make sure the model you picked accepts **image** input. MetaScrub sends still frames, so text-only models won't work.
- See the error table in [OpenRouter: API Key and Choosing a Model](OpenRouter-Setup#5-if-something-goes-wrong).

**Uploads stopped with a quota message.**
YouTube allows 10,000 quota units a day, and every upload uses some. The Schedule tab shows how many uploads you have left. The quota resets daily (midnight Pacific time). Queued videos wait until then.

**A channel says it's signed out.**
Open **Schedule** and reconnect it. If you'd turned on Discord alerts, you'll have had a "Something needs you" message.

**How do I remove MetaScrub's access to my YouTube account?**
Disconnect the channel in MetaScrub, or remove MetaScrub at [myaccount.google.com/permissions](https://myaccount.google.com/permissions). MetaScrub never deletes or edits your existing videos.

**How do I wipe everything MetaScrub stored?**
Delete the **Documents\MetaScrub** folder.

**Still stuck?**
Ask on **[Discord](https://discord.gg/HnqkyDkFUA)**.
