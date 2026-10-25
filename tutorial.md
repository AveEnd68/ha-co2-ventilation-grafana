Monitor CO₂ in your home office and get reminded to open the window

<HOOK – e.g. feeling tired after the third video call is often a sign of stale air, not of the meeting.> In this tutorial, you send CO₂, temperature, and humidity readings from Home Assistant to Grafana Cloud. You build a dashboard that compares your office with the outdoor air and an alert that tells you when it's time to open the window.

What you'll build

Dashboard showing CO₂ in the office with thresholds at 1,000 and 2,000 ppm, and indoor versus outdoor temperature and humidity

Before you begin

To complete this tutorial, you need:

Home Assistant <VERSION> or later, with administrator access
A CO₂ sensor in Home Assistant (this tutorial uses a <SWITCHBOT MODEL> via the <INTEGRATION> integration)
Optional: an outdoor temperature and humidity sensor
A Grafana Cloud account (the free tier is sufficient)
About <XX> minutes

This tutorial was tested on <DATE> with Home Assistant <VERSION> and Grafana Alloy <VERSION>.

Expose Home Assistant metrics

Home Assistant can publish sensor values in a format Prometheus understands. In this section, you turn on that endpoint.

<Action>.
<Action>.
yaml
   # configuration.yaml
   prometheus:
     <OPTIONS>
<Action>.

You should now see <VISIBLE RESULT>.

Create a long-lived access token
Connect Home Assistant to Grafana Cloud

For full details, refer to Home Assistant integration.

Find your sensor metrics
Build a CO₂ panel
Compare indoor and outdoor conditions
Create an alert rule
Test your alert
Troubleshooting
Symptom	Cause	Fix
<WHAT THE READER SEES>	<WHY>	<WHAT TO DO>
Next steps
To find out how long you need to air your room, refer to Analyze ventilation with a window sensor.
To get a reminder to close the window, refer to Set a window timer in Home Assistant.
To learn more about alerting, refer to Grafana Alerting.
References
Umweltbundesamt (German Environment Agency): Guide values for carbon dioxide in indoor air (<YEAR, LINK>)
<OTHER SOURCES>