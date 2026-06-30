# Now Playing — for Even Realities G2

Turn your **Even G2** glasses into a remote for whatever's playing on your phone.
See the app, track title, artist and progress at a glance — and control playback from the
R1 ring: play / pause, previous, next, and volume. Without taking your phone out.

**Android only.** Requires the free companion app **Media Bridge** (see below).

## What it shows

- App · title · artist · progress, right in your view
- Long titles scroll; live streams show **LIVE**
- A quiet **minimal mode** — just "Now Playing…" and a clock when you don't need the details
- Keeps working with the phone in your pocket, screen off

## Ring controls

- **Swipe** to move the cursor; **tap** to run the highlighted control (play / pause · prev ·
  next · volume).
- Controls stay hidden until your first tap, so a stray touch while walking won't skip a track —
  and they auto-hide after a few seconds.
- **Double-tap** is the back / exit gesture (on the play screen it repeats the highlighted
  control instead).

## Requires: Media Bridge (Android)

The glasses can't read your phone's media session directly — on Android, "what's playing" is only
exposed through a notification listener. So Now Playing needs a small helper, **Media Bridge**,
running on the same phone. It reads the active media session and serves it to the glasses over
localhost (`127.0.0.1`); **nothing leaves your phone.**

Media Bridge is free and open source — you can verify exactly what it does:

> https://github.com/r-tkbyc/takemotions-media-bridge

It registers an **empty** notification listener purely to see media playback — it never reads,
stores, or sends your notifications or messages.

## Try it

1. Install **Media Bridge** on your Android phone (link above), turn on *Enable media bridge*,
   and grant *Notification access*.
2. In the **Even App**, open **Prototype mode** and scan this QR (or open the link below):

![Scan in the Even App (Prototype mode)](QR_560962.png)

> https://r-tkbyc.github.io/even-now-playing/

3. Start playing something (YouTube, Spotify, a podcast…) and it shows up on the glasses.

Built and tested on Android with YouTube, Spotify and Amazon Music.

## Privacy

- Now Playing only reads what Media Bridge serves on localhost — your media info never leaves
  your phone.
- It requests **no special permissions**.

---

Made by **TakeMotions** · [@r_tkbyc](https://x.com/r_tkbyc)
