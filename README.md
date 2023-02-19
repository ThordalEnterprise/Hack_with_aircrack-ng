# Hack_with_aircrack-ng

_______Part #1 - aircrack-ng ______

-- Look for wifi --
airport -s

-- Look disable --
sudo airport -z

-- Sniff wifi interface + kanal --
sudo airport en0 sniff 6

-- Look for handshake --
aircrack-ng /tmp/airportSniffQ2qvVj.cap

-- Start crack --
aircrack-ng -w wordlist.txt -b 6A:41:47:CF:3E:9C /tmp/airportSniffQ2qvVj.cap

-- Make hccap --
aircrack-ng -b 6A:41:47:CF:3E:9C -J name  /tmp/airportSniffQ2qvVj.cap

-- Make hccapx --
aircrack-ng -b 6A:41:47:CF:3E:9C -j name  /tmp/airportSniffQ2qvVj.cap

_______Part #2 - Hashcat ______

-- Convert to hc22000 website --
https://hashcat.net/cap2hccapx/

-- Convert to hc22000 --
hcxpcapngtool -o hash.hc22000 -E wordlist dumpfile.pcapng


____________________
Test
____________________
