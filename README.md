# werejugo

Version 0.9 - beta

Identifies physical locations where a laptop has been based upon multiple forensics artifacts on host. Including

    - Wireless Profiles in SOFTWARE registry hive

    - Wireless SSID from WLAN_AUTOCONFIG Application Event logs

    - Wireless Diagnostic Event ID 6100 in SYSTEM.EVTX 

    - Wireless Profile Names from SRUM.DAT


To run this tool you need three files from this github repo.  Werejugo.exe  werejugo.yaml and template.html.  Download them and place them in a directory.

You must edit werejugo.yaml and give it some API keys. This tool requires that you provide both a wigle.net API key and a Google Geolocation API key.   Place those keys in the werejugo.yaml configuration file.  The google API key requires a credit card but the first several thousand requests per month are free so you can experiment with the tool with out incurring a cost.

Run the tool with administrative privileges on the target laptop for live aquistion of required files.  Auto file aquisition will only work on systems that have a version of esentutl.exe that supports extracting unlocked files.   If automatic acquisition fails then use another forensics tool to extract the locked files.

If you have a forensics image with unlocked files then you can browse to those files manually.

![](./werejugo.gif)

