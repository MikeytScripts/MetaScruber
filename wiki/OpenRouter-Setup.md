# OpenRouter: Getting an API Key and Choosing a Model

MetaScrub's **AI titles** feature needs an AI API key. [OpenRouter](https://openrouter.ai) is the easiest way to get one: a single account and key give you access to hundreds of models from OpenAI, Anthropic, Google, Meta, Mistral and others, and you can switch between them at any time.

This page covers the two things you need: **an API key** and **a model**.

---

## Part 1: Get an API key

### 1. Create an account

Go to **https://openrouter.ai** and click **Sign in**. You can use Google, GitHub or an email address.

### 2. Add credits

Open the **Credits** page from your account menu and add a small amount. **$5 is plenty to start.** You only pay for what you use.

Models whose ID ends in `:free` cost nothing, but they have tight daily limits and can be slow or busy. When you're scheduling a batch of Shorts, those limits run out fast, so use credits for regular use. Adding credits also raises the limits on free models. See OpenRouter's [FAQ](https://openrouter.ai/docs/faq) for the current numbers.

### 3. Create the key

1. Go to **https://openrouter.ai/keys** (account menu → **Keys**).
2. Click **Create Key**.
3. Name it something you'll recognise, like `MetaScrub`.
4. **Set a credit limit**, for example $5. That's the most this key can ever spend, so a mistake can't drain your balance.
5. Click **Create** and **copy the key straight away**. It starts with `sk-or-v1-` and is only shown once. If you lose it, delete it and make a new one.

### 4. Add it to MetaScrub

Paste the key into MetaScrub where it asks for your AI / OpenRouter API key, and choose your model (Part 2). MetaScrub's built-in **model browser** lets you search OpenRouter's models without leaving the app.

MetaScrub stores the key on your PC only, encrypted with Windows' built-in data protection.

**Keep it secret.** Anyone with the key can spend your credits. Don't post it in Discord, screenshots or support messages. If it ever leaks, delete it on the [Keys page](https://openrouter.ai/keys) and create a new one.

### 5. If something goes wrong

| Error | Meaning | Fix |
|---|---|---|
| 401 | Key missing or wrong | Paste it again, with no spaces. Check it still exists on the Keys page. |
| 402 | Out of credits | Add credits, raise the key's credit limit, or switch to a `:free` model |
| 429 | Rate limited | Wait a bit. Very common on `:free` models; adding credits helps. |
| 400 / 404 | Model not found, or it can't take images | Pick the model again from the model browser. Make sure it accepts **image** input. |

You can see every request and what it cost on OpenRouter's **Activity** page.

---

## Part 2: Choose a model

### The one hard rule: it must accept images

To write a title, MetaScrub sends **four still frames** from your video plus the file name and your channel's style notes. So the model **must accept image input** (sometimes called "vision" or "multimodal"). Text-only models will fail or write titles without seeing the video.

On **https://openrouter.ai/models**, use the input filter on the left to show only models that take **image** input before you pick anything.

### How model IDs look

Every model has an ID like **`company/model-name`**, for example `google/...` or `anthropic/...`. A `:free` suffix means the free, rate-limited version.

Models get new versions often, so copy the current ID from the model's page (or pick it in MetaScrub's model browser) rather than typing it from memory.

### What to compare

| Thing | What it means | For MetaScrub |
|---|---|---|
| **Image input** | Can it see pictures? | **Required** |
| **Price** | Per million tokens, split into **input** (what's sent: the frames and your notes) and **output** (what it writes). | Input matters most here, because images take up a lot of tokens. Titles are short, so output cost is small. |
| **Speed** | Tokens per second and latency, per provider. | Small "mini", "flash", "haiku" or "lite" models are fastest and cheapest. |
| **Context length** | How much it can take in at once. | Anything modern is plenty. Four frames and some notes are small. |
| **Quality** | How good and on-brand the titles are. | Bigger models follow style notes better and write punchier hooks. |
| **Data policy** | Whether the provider stores or trains on what you send. | Check this if your videos aren't public yet. You can restrict providers in your OpenRouter privacy settings. |

### What to pick

| You want... | Choose... |
|---|---|
| **The best starting point** | A small, cheap model from a big lab that accepts images (look for "flash", "mini" or "haiku"). Fractions of a cent per video, fast, and good at short catchy titles. |
| Better titles, and you don't mind paying a bit more | A flagship image-capable model from near the top of [openrouter.ai/rankings](https://openrouter.ai/rankings) |
| To try it for free | An image-capable model with `:free` in its ID. Expect limits and busy errors on big batches. |
| Titles in a language other than English | A larger model. Small models are weaker outside English. |

### A simple way to choose

1. Filter models to **Image** input and sort by price.
2. Pick two or three candidates: one cheap, one mid-range, one flagship.
3. Schedule the same few videos with each, with **Approve titles before upload** turned on in Post settings, so nothing goes live while you're testing.
4. Keep the cheapest one whose titles you'd actually post.
5. After a day of normal use, check the **Activity** page to see what it really costs per video, and set your key's credit limit to match.

You can switch models at any time. Nothing else in MetaScrub changes.
