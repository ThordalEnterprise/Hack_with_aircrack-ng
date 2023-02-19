# Hack_with_aircrack-ng

This process describes a set of commands used to crack a WiFi password using two different tools, aircrack-ng and hashcat. The process involves the following steps:

Part #1 - aircrack-ng:

- Look for available wifi networks.
- Disable wifi.
- Sniff wifi packets on a specific channel.
- Look for the password handshake of the target network.
- Start the cracking process using a wordlist and the captured password handshake.
- Convert the captured handshake file to hccap or hccapx format, which is compatible with hashcat.

Part #2 - Hashcat:

- Convert the hccapx file to the hc22000 format using an online converter or hcxpcapngtool command.
- Use hashcat to crack the password using the hc22000 file and a wordlist.

It is important to note that these tools should only be used for ethical purposes and with the consent of the network owner.
