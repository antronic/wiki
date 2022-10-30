We have a YouTube channel at <https://youtube.com/@creatorsgarten>. They are for publishing talks VODs.

Meanwhile, live stream archives can be found on the [Creatorsgarten Facebook page](https://www.facebook.com/creatorsgarten/videos/).

# Common audio/video issues

For livestreaming:

- Audio too quiet. Check in OBS that when speaking, the sound level is in the yellow color zone [between -20 and -9 dB](https://www.reddit.com/r/Twitch/comments/nctu56/best_sound_levels_for_obs/)

- Audio output works in one channel only. Check in OBS and make sure that there are 2 volume bars (left and right channel). If the problem from the source cannot be fixed, go to Advanced Audio Settings and make it mono.

For preparing VODs:

- Video and audio not synchronizing. In a video editor software, detach the audio from video, so that they can be moved independently.

- Issues that interrupt the presentation. For example, connectivity problems, technical issues. They might be safe to cut out from the VOD.

# VOD preparation

- [Work on preparing VODs are being coordinated on Airtable.](https://airtable.com/shru5fGOzjhHHxo05)

- Each talk goes through several stages before they are published to the YouTube channel.

   1. **Source** — Obtain the source material, either recorded in OBS, or downloaded back from Facebook Live.

   2. **Timestamp** — Determine the time range within the source material that contains the talk.

   3. **Slice** — Cut the source video around the time range and put it in its own file. This results in a smaller file that’s easier to work with.

        The [`cut`](https://github.com/creatorsgarten/videos/blob/main/bin/cut) script can be used to cut the video in a lossless manner using ffmpeg.

- Supporting code lives in [creatorsgarten/videos](https://github.com/creatorsgarten/videos) repository.

- If you’d like to help, you can find us [in the #📼-vod channel on Creatorsgarten’s Discord server](https://discord.gg/mVX8yEdhWX) and mention to “@VOD Team”.