# minemoji-pack
Minemoji Pack Template

## How to?

- Make your own repo from this template 
- Enable github pages (with github actions selected)
- Edit `.github/workflows/pack.yml` to change the PACK_NAME.
  - This will change the 'prefix' used for your emote pack.
- Clone repository OR Upload files to site
    - Files are uploaded to the assets/ folder.
- When you're done, commit your changes.
- After a few moments your emote pack should be ready! (obvs, replace the pages url and pack name below. if you dont know your pages url, go to Settings -> Pages)
    - Resource pack: `<your pages url>/<PACK_NAME>.zip`
    - Emote json: `<your pages url>/<PACK_NAME>.json`
- You shouldnt need to do anything with the resource pack file. Just put the emote json in your minemoji/config.yml, under custom-packs: packs: (see example config below)


## Example Minemoji Config

```
unicode-emojis:
  enabled: true # default option, set to false to disable default emojis...
  uri: "https://itscinnamon.dev/minemoji/packs/twemoji-latest.zip" # If URI is omitted while enabled, it will be presumed to be bundled in another pack.

custom-packs: # Packs can be placed in either minemoji/packs or put in the following "packs" list to be downloaded.
              # This is useful for packs from external sources :)
  packs:
    - "https://itscinnamon.dev/minemoji/packs/minemoji-latest.json" # Minemoji example pack
    - "https://itscinnamon.dev/minemoji-template-pack/minemoji.json" # Template
    - "<YOUR GITHUB PAGES URL>/<PACK_NAME>.json"

enforce-pack: true
# use minimessage!  :) remove entry to disable prompt
join-prompt: "This server uses resource pack to allow players to use emotes in gamechat :) <click:open_url:'https://github.com/cinnamondev/minemoji'><u><b><aqua>About</aqua></b></u></click>"
```

## Note

The images in this template pack are not my own-- they are here for demonstrative purposes. 