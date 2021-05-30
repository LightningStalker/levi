# Beacon Levi
Programmable ATtiny85 CW keyer

- Uses Digispark library
- Small form factor
- USB serial programmable
- DC 5-30V (With regulator on Digispark)
- Configurable 5-20 WPM+
- 510 character message storage (EEPROM size - 2)

## Usage
1. Program using Arduino IDE. You may need to install the Digispark libraries.
2. Start serial monitor
3. Jumper modePin to ground (default Digispark pin 0)
4. Plug in or reset Digispark
5. Unfortunately due to a bug in the software USB serial library, you must wait a for fullstops and garbage characters to stop appearing. This may take over a minute in some cases.
6. Press the open bracket key '['
7. The 3 above steps may take several tries unfortunately. It should however start working. I would fix the affected libraries myself however I feel that is the job of the maintainers.
8. You should see a prompt for wpm. 1 is 5wpm, 2 is 10wpm and so on up to 20wpm. Other input is ignored and set to the default of 5wpm.
9. Type your alphanumeric message followed by a close bracket ']'
10. You should now see your entered information read back to you for confirmation.
11. Reset, remove the jumper and your message should begin wandering out of keyPin as morse code and the LED on the Digispark should flash. Default is Digispark pin 1
12. Quince Johnny Adamsson
