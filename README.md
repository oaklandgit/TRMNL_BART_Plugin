# BART Departures Plugin for trmnl

This is the code for a trmnl plugin that fetches upcoming departure information for a station you choose. It leverages this BART API along with a public key available from their site.

https://api.bart.gov/api/etd.aspx?cmd=etd&orig={{trmnl.plugin_settings.custom_fields_values.from}}&key={{api_key}}&json=y
