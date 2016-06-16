# USB-CAN-Adapter
I've bought a usb2can adaper on some china's online market (meny vender offers it). But the software included doesn't work, or It was written in Chinese language. I would liko to write another one in English language to everyone.

How I did it:
I've sniffed the original program ( with a free see attached files) with free comm sniffer tools (http://www.hhdsoftware.com/). Very nice tool, I suggest it!
In this way, I've seen that:

Every pachet on COMM start with 0xAAAA, 4 byte with ID, 8 byte data, 1 byte empty.
Then 1 byte at 0 for ID at 11 byte or at 1 for 29 extended ID.
Then again 1 byte for RTR.
Here a checksum (without AAAA), a simply sum, then the end with 0x5555.

Initiaslly, I''ve wrote a, .hta test program, then another with an advanced COM handler (MSCOMM32.OCX). Here I post the 1st.
It was usefull the use of PCAN sniffer. I'm unenploied, so my frend give it to me...

Then, I?ve wrote a C program using the old Borland c++ Builder 6 (the two china's program was written in the same way, or in Delphi).

I'm here to shere my job, ideas and contribuite to make a 20$ sniffer more efficent.

P.S.: If someone have the original firmware software I?m very happy to handle this and correct/rewrite the new one.
Also, the scheme can help me to rewrite a new firmware, with the suggestion/help of other users.
