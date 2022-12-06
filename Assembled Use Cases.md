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
- A report page which requires a captcha
- handle scores
  - and deleting the scores, verifying that they exist, fetching all the forms etc.etc.etc.
- For searching and archives have a temporary page that does the bare minimum
  - Will be replaced by hybrid archive search service later
- wl token verification and info
-    
