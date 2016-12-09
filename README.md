# openwrt-traffic-emulator
OpenWRT traffic emulator frontend


These little scripts will provide a frontend to emulate network condition for mobile app testing. The backend cgi use tc qdisc to setup Traffic sharping condition for limit bandwidth, loss and latency.
Inspired by this package: https://github.com/shuhaowu/trafficcop

But the trafficcop package does not work on TP-link MR302 device and provide no custom input for loss, latency and bandwidth so this script provide simple method.

-- How to setup:

On openwrt shell: install uhttpd, tc and kernel module: kernel-sched
Clone repo and migrate traffic, reset to /www/cgi-bin 
