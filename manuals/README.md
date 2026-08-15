

My question will give away my lack of knowledge but here goes...

When switching bands with the Ultimate 3S the Low Pass Filters if mounted on a Relay Filter board are selected by the control unit (0 thru 5). I see no provision to select matching band pass filters other than by plugging/unplugging each BPF module. Is it possible to use a second relay board to select the proper BPF as well? Will the control unt supply enough current to operate both relay boards?

Got my receiver kit yesterday and I am expecting the final pieces, the case, in the next few days. Can't wait to get started with the build.


73,

PJH, N7PXY

Reply
Like
More
09/14/16  #11264  
Hans Summers

Hi Patrick

Yes, it is possible. The size and pinout of the BPF board is identical to the LPF board - for this reason.

Yes, the AVR output will support the two 28mA relay coils in parallel. AVR outputs are capable of more than most people realise and the facts are very well-buried in the hidden corners of the datasheets. But it WILL work. 

You will need to do some wiring between boards etc., it won't all just plug together easily. The receiver PCB does not have a slot for a relay, the way the main U3S PCB does. So it would be limited to 5 band switching, not 6 - unless you cut some tracks and mount the 6th relay on another matrix board or whatever. 

A separate difficulty will be how you inform the WSPR decoding PC what band the receiver is on, so that it uploads correctly to WSPRnet. I understand WSJT-X version of the WSPR decoding software does include a facility for stepping through bands automatically - and it may be possible to set up a U3S with the same matching schedule so that even without any actual synchronising communications between U3S and PC, it will still step through in the same sequence. 

If you do it please inform us, so we can all learn from it!

73 Hans G0UPL
http://qrp-labs.com

