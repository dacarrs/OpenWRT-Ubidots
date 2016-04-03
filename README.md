# OpenWRT-Ubidots
OpenWRT ping respone time monitoring to Ubidots

Requires luci-lib-json, install on OpenWRT router with:
opkg update
opkg install luci-lib-json

Upload the ubidots_ping.lua to /usr/lib/lua
Give execution permissions with: chmod +x /usr/lib/lua/ubidots_ping.lua

To post ping response time to Ubidots:
/usr/lib/lua/ubidots.lua -post <API_Key> <Device_ID>

Replace <API_Key> and <Device_ID> with your values.

Help can be obtained with /usr/lib/lua/ubidots.lua -help

Based on https://github.com/ediy/Ubidots-Lua-OpenWRT-router-Ubidots-Real-time-data-monitoring and modified to 
post only ping respone time.
