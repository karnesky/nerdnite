# Nerd Nite Water Color Map Generator
## What is this?
An ugly "first pass" to generate beautiful maps of [Nerd Nites](nerdnite.com).
## How do I use it?
As noted above, it is a bit ugly, but here's what you do:

1. Copy `stamen.html` somewhere local
2. Download a local copy of [nerdnite.com/nn-api/cities](nerdnite.com/nn-api/cities) to a file named `cities` in the same directory. Techy-geeky stuff: We do this because the remote nerdnite.com host doesn't have cross-origin headers to allow you to use it and I don't believe the API generates JSONP that would allow this. I also don't think we have [CORS](enable-cors.org) on the server.
3. Open `stamen.html` in Firefox. It may work in other browsers. It may not.
4. Wait. A while. Techy-geeky stuff: Map generation is intentionally HORRIBLY slow. This is because we look up long/lat from city names where bosses haven't entered their info. Google hates when you do this too often, so we throttle this to some minuscule rate.
5. Take a screenshot and crop it and you're done.

## Credits
This is ugly, but the tools that it uses are not.
Props to Dan for the Nerd Nite API and to [Stamen](maps.stamen.com) for the
great tileset!
