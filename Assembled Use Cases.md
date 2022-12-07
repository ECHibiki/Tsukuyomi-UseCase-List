# Assembled

## Moderator Tools
- Be able to disable captchas on forms
- Configure a blotter and put the blotter into an API file for each board
- Flexible combination of setting poll boards which can have no polls
- Setting a board as a Scoreboard
- Setting a board as a fileboard
- Embeds should be allowed to be spoilered from the mod UI
- Add a new poll option for rank order voting(radio, multichoice, ranked)
- Allow mods to upload or remove files in the static directory
- Modify the properties.json files which control pages
- Modify Featured pages 
- Set the message of the day txt from dash
- Edit a poll

## Server Operations
- Create a flexible interface to create thumnails with imagemagik or another alternative
- Create exif stripping on mp4, png or jpg to only remove personal/GPS data and leave other info intact.
- /all/ does not need to be rebuilt on certain threads identified as hidden
  - Hidden needs to be a flag which prevents a board from listing in /all/, summaries and home 

## User Tools
- Embeds should be allowed to be spoilered from post
- Submit a score for score update
- View scores on posts from the API or HTML display
- Submit a vote on a poll for radio/multi/ranked
- Thumbnail inputs on video content should set a timestamp
- A page should exist which displays user IP, Hostname, agent
- Filter systems that handle a wide range of cases
  - see filters.php for full list
  - should be set in config settings for bans, captchas and rejections
- A public ban listing for users to know what's getting banned
  - Reduced functionality
  - Show a post and the reason it was banned, the board and duration
  - No other info is needed
  - see https://4chan.org/bans as an example
  - If I need to list them all then it will be paged
- Have a page for ban check that's blocked by captcha 
- A page which takes post data and builds a ban message from it.
- Transition page for cycling between new and old UI via cookies
- Handle polling inserts
  - and deletes and creates and get data and formatting for DB insert etc.etc.etc.
- handle scores
  - and deleting the scores, verifying that they exist, fetching all the forms etc.etc.etc.
- For searching and archives have a temporary page that does the bare minimum
  - Will be replaced by hybrid archive search service later
- wl token verification and info

- Deleted/Cyclical posts should go into archival state which places files into recycling
- Deleting files are moved into recycling to be retrieved if restored. 
  - Recycled items are deleted based on last modified time.
- User deletes to be done effecting scores or polls
  - File deletions and post deletions and embed deletions
- A report page which requires a captcha
  - Block banned users from submitting
  - Have a user limit so submitting
  - Add report to the mod list
  - send emails
  - Do Spam checks
- Appeal
  - Verify existing appeal
  - Check if ban is appealable
  - Send appeal
  - Do Spam checks
  - Show user that appeal has been sent.

- On post check for board locked
- Process input post issue
  - verify errors
  - Format polls if exists
  - Set spoiler value, frame
  - check if it's an OP
  - Donor states
- Verify there's no post input flooding going on (after image verifications)
- Check up submission 
- Do ban, DNSBL, text filter, OCR checks, Blockhash and Board Specific checks
- Low mod activity checks and settings that go off if there's no mod access recorded
- Building the citations table and any other text reading database updates
- Inserting data into the database
- Inserting images in such a way that a custom CDN imageserv could be used
- Add a flood post for filter triggers
- Cyclical, bump, (no)noko and zombie handling
- Building HTML pages (also the 50 post only versions)
- Building API pages (the works from hazuki)
- Some actions should occur in the background since not all themes should be built
- The routes that the building of API or HTML pages can be varied based on the page style being used(kissu vs original ui)

- When filters are triggered, store a temp post to the DB with the tmp file stored somewhere
- Captcha release to verify captchas sent
- On captcha release pull out a stored image and data
  - Will have to perform OCR checks and do a hard reject on fail
  - Text filters should all be pre verified
- On release do the post-filter actions of standard posting. 
