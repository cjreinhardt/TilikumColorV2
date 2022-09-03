# What color is Tilikum Crossing right now?

This website will attempt to show you the current color of the Tilikum Crossing Bridge in Portland, OR. A

According to [this article from Multnomah County](https://blog.trimet.org/2016/03/21/how-it-works-tilikum-crossing-art-lights/), the color of the bridge is largely based on the water temperature of the Willamette river. 

First this page checks to see if it's daytime in Portland (using [SunCalc.js](https://github.com/mourner/suncalc)). If it is, we list the color as 'Gray'. If it's nighttime we fetch the most recent water temperature reading from the [closest USGS monitoring station to the bridge](https://waterdata.usgs.gov/monitoring-location/14211720/#parameterCode=00065&period=P7D) in your browser/clientside.  Based on that temperature we devise what the likely color of the bridge will be based on some previous data i've collected. It's very possible it will be wrong, but this is just for fun, right? 

Here's what you'll need if you want to get this running locally:

Prerequisities:
- Not much, it's just HTML, CSS and JS!
- Since i've been hosting it on Netlify, i've been using the Netlify CLI to start up a dev server locally.

1. Clone this repository
2. Open the root directory of the cloned repository in a terminal.
3. Run 'netlfiy dev' to start your local server.
6. That's it!  

If you want to deploy it to Netlify commit your changes to a new repository and [connect it to Netlfiy](https://docs.netlify.com/configure-builds/repo-permissions-linking/), should work without much fuss!