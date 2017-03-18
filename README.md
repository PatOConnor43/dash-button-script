# dash-button-script
A simple script to validate that an Amazon Dash Button is being pressed on your network.

This script depends on you knowing what the MAC address of your button is. This can be done fairly simply by using Wireshark.
All you need to do is start Wireshark and filter for ARP requests. If the dash button is set up to connect to your network,
when you press the button you should see a new ARP request from an Amazon device. You can paste your MAC address from that into
the `dashbuttons.register()` call.
 
