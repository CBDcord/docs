Planned features:

- Music bot (private feature not for distribution)
  - Commands:
    - Queuing songs
    - Place a song at the start of the queue
    - skipping a song
    - repeat current song
    - Pause/resume
    - Volume up/down
    - create playlist from queue
    - View all songs previously played/queued from current listening session
    - Shuffle the queue
    - Leave the VC
    - Lyrics
  - Integrations:
    - Discord slash commands
    - Web interface (Discord SSO)
    - Save created playlists to Spotify account
    - Play songs from Spotify playlist
    - Queue songs from [REDACTED] or SoundCloud via link or title
    - Persist queue to database
- Event counters
  - Simple word counting
    - Count the number of times a specific phrase is typed in the Discord server
    - Allow users to add counters for any phrase
  - User invoked counting
    - Allow users to record when an event occurs such as a bruh moment
    - Let the user select the:
      - counted word
      - trigger word
      - response phrase
      - name of the counter
    - Store all counters to database
    - Fetch total # of events or # of events caused by a specific person
- Moderation features (might use AWS step functions and offer as paid feature):
  - Abstract moderation actions into workflow steps that can be arranged into complex workflows
  - Build web interface to allow server admins to configure workflow steps. Allow steps to be drag and dropped in any order
    - Workflows will be similar to IFTTT or IOS shortcuts. Allow output of one workflow step to flow into the next as the input
    - Configure workflows to be triggered via a custom trigger word, emoji, web interface button, or CRON schedule
