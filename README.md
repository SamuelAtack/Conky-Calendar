# Conky-Calendar
A clean Conky desktop widget for Linux displaying system stats and Google Calendar.

## Features
- System info: CPU, RAM, swap, disk, and network usage
- Top 5 processes by CPU
- Live Google Calendar week view via gcalcli
- Teal and white colour scheme with today's date and current events highlighted in orange
- Auto-starts with the desktop session

## Dependencies
- conky
- gcalcli (authenticated with your Google account)
- Ubuntu Mono font

## Setup
1. Find your network interface: `ip link`
2. Replace `YOUR_NETWORK_INTERFACE` in `.conkyrc` with your interface name (e.g. `wlp0s20f3`)
3. Authenticate gcalcli with your Google account: `gcalcli init`
4. Copy `.conkyrc` to `~/.conkyrc`
5. Copy `conky-cal.sh` to `~/conky-cal.sh` and make it executable: `chmod +x ~/conky-cal.sh`
6. Copy `conkystart.sh` to `~/conkystart.sh` and make it executable: `chmod +x ~/conkystart.sh`
7. Add `conkystart.sh` to your startup applications
