# Xbox_Bench_Psu
My first Hackatime project 

Yes, this was a one day project.
Lapse link:  https://lapse.hackclub.com/timelapse/OsR8z70i6DGW

Journal:

After my xbox 360e died from a lightning strike (long story short, 3.3v rail was fried), it no longer could give the go ahead to ramp up the PSU input from 5v to 12v.
That got me thinking. So a little digging later, I found there was 0 smart negotiation, console just pulled the 5v standby and the sense wire together, and boom, you get 12v. 
So after cracking open the barrel jack i found that since this was a aftermarket supply, the wires were not what i expected them to be coloured. With a mixture of guesswork and continuity testing as seen in the timelapse, I more or less figured out the pinout of the barrel jack. 
<img width="3024" height="4032" alt="IMG_9825" src="https://github.com/user-attachments/assets/cf88ee04-1e38-4659-aa33-bc4c8e58e272" />

I say guesswork, because to be honest, process of elminiation could have got me there too. The red and black wires were obviously a much fatter gauge, which meant they were primary 12v rail so as long as i tied the two smaller wires together, it didn't matter which was sense and which was 5V standby, it would have worked anyways. But whatever lol. 

So anyways i got cracking, soldered the white and green wires together, tinned the wires and stuff, and since this is a high current application, i chose the x4016LE, a 8A buck.
This one's given me some pain in the past, trying to power a Pi5, but for our purposes it should be fine. So anyways back to it, because it was a high current application, i decided the screw terminals weren't gonna cut it, so soldered to the PCB it was. (Yoda? is that you?). Anyways at the end of the lapse, you can see i fired it up did some multimeter testing, powers a 12v fan from the same dead Xbox. Also the voltage step down does work, and the fan slows when you decrease the voltage (duh) . Anyways, it was a quick project and i gotta go study for exams instead of messing around. Bye!
