This plugin provides DNS Ad Blocking support to the Gargoyle Router Firmware.
The block list automatically updates every Sunday at 4:00am.

Install
- Refresh plugins
- Install "DNS adblocking support for Gargoyle"

Updating

To update the plugin, first uninstall it, then install the new version
- For the latest version, add the following as a feed in your System->Plugins page
"http://lantisproject.com/gargoyle_plugins"

Verify the plugin is operating correctly

Visit the page: http://ads-blocker.com/testing/
If you can't see any ads, you're good to go. If you are seeing ads, your computer may be loading a cached version of the site which includes the ads. Try clearing your cache (CTRL+F5 refresh the page).

Black List

Used to add sites to the block.list that are not already included.

White List

Used to remove sites from the block.list. 
NOTE: The white list will ONLY remove items that are ALREADY ON the block.list. If they aren't on the list, don't bother white listing them.


CHANGELOG

Version 1.1.0
- Added GUI for interfacing with the block, black and white lists
- Added transparentpixel.gif file to the plugin so we no longer need to retrieve it from a remote source
- Reworked plugin so that it installs to "/plugin_root/". This means that the plugin installation will now respect the use of external usb storage automatically.
- REMOVED: legacy web server support (httpd_gargoyle)
- REMOVED: wireless_only capability, gargoyle bridges the wifi and lan networks causing this functionality to break. If someone has an idea for fixing it, i am happy to add it back.

Version 1.0.4
- BUGFIX: Fixed incompatability with the DDNS plugin

Version 1.0.3
- BUGFIX: Fixed incompatability with the Tor plugin
- Fixed localisation strings for ZH-CN and RU

Version 1.0.2
- Fixed localisation strings for time of last update (Thanks Obsy) and PL language file
- BUGFIX: Crash on small memory devices (minor change to how the ad list is retrieved, now uses half the space during setup). End result is still the same. Not a necessary update if you weren't experiencing any problems previously.

Version 1.0.1
- Added German, Norwegian, Polish, Russian and Spanish translations
- Added documentation for how to use the black/whitelist functionality (front end for this will be in a future release)
- Added documentation about how to test the plugin is functioning correctly
- BUGFIX: Workaround for browser based ad-blocking plugins detecting this plugin as malicious, breaking the plugin (Thanks Eric).

Version 1.0
- Initial release
