# Shots Fired

Shots Fired is an [Overwolf app](https://www.overwolf.com/) that helps to automate scene switching and source item visibility within OBS.

It was developed as part of the [PUBG Developers Challenge](https://play.overwolf.com/pubg-dev-challenge/).

![](https://cldup.com/VJ48vOLCkW.png)

# Usage

## Connecting to OBS

1. Shots Fired requires [obs-websocket](https://github.com/Palakis/obs-websocket/releases) to enable automation. Choose the latest Windows installer and follow the instructions.
2. After setting up a password in OBS (`Tools > Websocket server settings > Enable Authentication (checked) > Password`), enter the same password into Shots Fired
3. The address field should remain as `localhost:4444` unless you changed it in OBS
4. Click `Connect` to continue.

[Show me how this works](https://www.youtube.com/watch?v=Dty4k_zGA74)

## Using Shots Fired

A mapping is a 1:1 connection between an in-game event (i.e. `jump`, [see: all events](http://developers.overwolf.com/game_events_status/game_events_status/)) and an OBS `scene`.

Each OBS scene has one or more sources, for example:

![](https://cldup.com/WXlGqnEXiQ.png)

When choosing a scene, Shots Fired will list all the sources and allow you to select which ones should be visible using the hidden/visible toggle:

![](https://cldup.com/Uj826wO2CE.png)

At this point, you may also optionally choose to add a delay and duration. Both are measured in seconds.

![](https://cldup.com/HREV9p6SwA.png)

A `delay` will add time before the source is shown. I.e. If a `jump` event has occurred and your `delay` for a source item called `jump animation` is set to `3` - there will be 3 seconds that pass before OBS shows `jump animation`.

A `duration` will hide a source item after the number of seconds has passed. I.e. If your `jump` event has a delay of `5` - the `jump animation` source will run for 5 seconds before hiding.

If you don't provide a delay, or it is set to `0` - the source is shown as soon as the event occurs.
If you don't provide a duration, or it is set to an empty value - the source will show indefinitely.

After saving you can preview how the mapping will look by clicking the play button, alternatively you can edit or remove the mapping.

![](https://cldup.com/QNQlb0wqHL.png)

If you would like to temporarily disable any mapped events from triggering changes, you can change the toggle state in the game header from `on` to `off`:

![](https://cldup.com/kuAqHl3XPc.png)

[Show me how this works](https://www.youtube.com/watch?v=g3Cr5wn0eKg)

# Support

If you've found a bug or would like to suggest a feature, [please raise an issue](https://github.com/artdevgame/shots-fired-support/issues).
