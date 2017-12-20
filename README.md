**DESIGN**

It's a keychain sized little PCB, with a built in antenna on one side, and the NFC chips and buttons on the other.
This little device sports two beefy NFC chips, each with 8KB of storage capacity. This is way way bigger than most NFC tags out there.
I've set it up so both chips work with the single antenna, and you need to press a button to activate it. You press the left button, you get the contents of the left chip, and press the right for the contents of the right.
When neither buttons is pressed, the circuit from the antenna to the chips are broken, and it's physically impossible to passively read it's contents.
The antenna itself was designed using this useful online generator, and it has enough inductance to run one chip at a time. It's also intentionally tuned just outside of the 13.56MHz NFC standard, for security, so you have to basically place the tag directly on top of the reader for it to work.
Heatshrink covers the outside, and helps protect the components, for when it's in your pocket or whatever, just like the Open Dime.

[Antenna Generator](https://kbeckmann.github.io/nfc-antenna-generator/)

*I don't have an Iphone to test on, but it works well on all the NFC capable Android phones and tablets I've tested.*

**USE-CASES**

The original use case I had in mind for this was for sharing GPG public keys in person. The two 8KB chips are pretty well suited for this kind of thing, and are big enough for most key lengths.
Outside of that, you have the standard door entry systems, personal business card type applications, bitcoin addresses etc. Some bitcoin ATMs use NFC, so it might be useful there, plus I've also seen people clone their tap-to-pay credit cards, and the activation buttons on this could make it a little more secure in terms of stopping passive activation.

**OPEN SOURCE**

As always, all of this is open source, so if you want to build your own, the PCB files are in a new github repo.
Besides the boards, you'll need the following components:
- 2x STMicroelectronics M24SR64-YDW6T 8KB RFID Chips
- 2x 4.5x4.5x0.5mm 4 Pin Momentary Switch
- Heatshrink Tubing (optional)


So that's the NFC Key, a simple little project. Hopefully some of you will find it useful. Thanks for watching, and I'll see you in the next video.

[Github Repo](https://github.com/N-O-D-E/NFC_Key)

**AVAILABLE SOON**

[https://N-O-D-E.net/shop](https://N-O-D-E.net/shop)

--
***BY NODE***
