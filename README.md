# Wizctl
Control [WiZ](https://www.wizconnected.com/en-us/products/bulbs) smart light bulbs through the CLI. This should work on most bulbs, although the actual features available may vary.

# Dependencies
- sh-compatible shell (e.g BASH)
- [Netcat](https://netcat.sourceforge.net/)

Before using this script, you need to first connect the light bulb to an accessible network connection. Also, you must know the IP address assigned to your light bulb. You can find it on your router's settings page or through the official WiZ application (some have mentioned, but I personally couldn't find it there).
# Install
Download the [wizctl](wizctl) script and put it under `$PATH`.

# Usage

Options (can be passed together on one run):
- Show help: `-h`
- Set IP address: `-a <IP ADDRESS>` (you should pass this option when first running the script; the IP will be saved automatically for later use)
- Set state (on/off): `-s <on|off>`
- Set light color temperature: `-t <TEMP>`
- Set light intensity (dimming): `-d <DIMMING>`

# Environment Variables

Override the `WIZ_IPFILE` variable prior to running to set a custom path for the IP address.

# Missing Features

- [ ] RGB Color
- [ ] Set a scene
- [ ] Getting current state

# Credits
- [UDP code reference](https://seanmcnally.net/wiz-config.html)
