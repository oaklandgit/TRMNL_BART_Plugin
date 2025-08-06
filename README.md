# BART Departures Plugin for the TRMNL E-Ink Dashboard

<img width="800" alt="CleanShot 2025-08-06 at 06 41 19" src="https://github.com/user-attachments/assets/cd16c414-d693-4c3f-917b-72afd77d1e7d" />

This is the code for a trmnl plugin that fetches upcoming departure information for a station you choose.

It leverages [BART's Legacy API](https://api.bart.gov/docs/overview). Specifically, it calls their Real Time Departures (RTD) endpoiont like so:
```https://api.bart.gov/api/etd.aspx?cmd=etd&orig={{trmnl.plugin_settings.custom_fields_values.from}}&key={{api_key}}&json=y``` where ```trmnl.plugin_settings.custom_fields_values.from``` is populated by the user's selection (defined in the yaml file).

The API key is available from BART's site at [https://www.bart.gov/schedules/developers/api](https://www.bart.gov/schedules/developers/api)

Definitely some issues to iron out as I'm getting familiar with the odd quirks of the TRMNL's templating engine. But more importantly is figuring out how to make the departure times accurate, given the way TRMNL pulls and caches its fetches. Stay tuned (or help out!)




