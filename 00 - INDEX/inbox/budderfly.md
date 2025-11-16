# Budderfly

On board devices in QA:
fsgqa2installer.budderfly.com

## MQTT Brokers URL
'DEV':  "a27jytqhlhczcs-ats.iot.us-west-2.amazonaws.com"
'QA':   "a14nq677yhks79-ats.iot.us-west-2.amazonaws.com"
'PROD': "a1slgwp6lsrlw9-ats.iot.us-west-2.amazonaws.com"

## MPA
MPA0: 08-d1-f9-58-33-ec: Original one in the pilot store, wire desoldered
MPA1: 08-d1-f9-58-34-7c: Ezurio could be flashed but not comunication with ESP32
MPA2: 08-d1-f9-58-33-e0: Ezurio TX and RX shorted

## MPA commands

Reset device after 3 seconds
HEX:    00 00 81 04 00 B8 0B 00 00
BASE64: AACBBAC4CwAA

Send connections events
HEX:    00 00 82 00 00
BASE64: AACCAAA=

Send connections events with monitor ID
HEX:    00 00 82 0D 00 31 32 33 34 35 36 2D 71 77 65 72 74 79
BASE64: AACCDQAxMjM0NTYtcXdlcnR5

Send connections events with monitor ID
HEX:    00 00 82 24 00 30 37 38 66 63 61 37 65 2D 66 39 32 66 2D 34 38 65 66 2D 61 30 30 31 2D 37 33 36 38 34 36 39 39 35 65 61 65
BASE64: AACCJAAwNzhmY2E3ZS1mOTJmLTQ4ZWYtYTAwMS03MzY4NDY5OTVlYWU=

Activate debug
HEX:    00 00 83 01 00 01
BASE64: AACDAQAB

Deactivate debug
HEX:    00 00 83 01 00 02
BASE64: AACDAQAC

Clear debug
HEX:    00 00 83 01 00 03
BASE64: AACDAQAB
