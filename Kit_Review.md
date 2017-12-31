I got this amazon gift card from work and had already done my holiday shopping right before black Friday ... guess what I did!

TLDR

Edited: dropped to 3 star after fiddling with the bed, felt that too many small issues, and a one or two big ones are annoying me.  I also had one great experience with support.

Edited: But then I also have unresolved issue on another part and a completely different support experience.   gave up and self-fixed that with my own purchase, now 2 stars. 

I feel it is wise to call out the two parts that are now non-stock:

1. Hotend extruder feeder is now a different mechanism and does not slip.  RRG did me right.
2. Heatbed:  I couldn't get support this addressed.  I was advised to not use current Marlin firmware, and advised later to zip-tie the cords.   Even though the thermistor wires detached themselves.  And the board resistance is 1.6Ohm which (by my understanding high).  The board did not heat evenly either (see picture).   For this I ended up self-fixing with an unplanned upgrade.  The heatbed is now a [[ASIN:B075375HBY Anycubic Ultrabase with MK3 Heatbed]] and controlled by a [[ASIN:B01HEQVQAK BIQU Heat Bed Power MOS Tube]].  The latter just avoids the RAMPS board and its 11A current limit and will allow me an easier path to change that board over to 24V with a new power supply.

Those two targeted changes in (me, now in another $40 or so) I'm at a good place with the printer.

==== DETAILS ====

Buy it if you are relatively confident in tinkering and willing to accept having to figure out whether you are facing a part problem, build problem, or calibration issue.

Overall: “B- or C+”

I think its a okay kit with some issues.  Those issues will be due to working with generic mass produced parts that may or may not work for you.

Parts: I did find some issues with my parts that needed revision. Most (all) parts a generic ones you will find for DIY kits on 3d forums, etc.

Completeness: This is a good functional printer, but lacks some of the nicer touches other kits have such as auto-leveling and a good quality filament spool.

Documentation: Build manual is most of the time easy to follow, but it references older iterations of the hardware which makes things such as the “bill of materials” not quite match up with the current kit. It also ends abruptly without providing advice on how to get to your first successful print after getting the software installed.

Software: Open Source and Open Source software. The newer slic3r and (look for the Prusa Slic3r build) are really quite functional.

Service: I have exchanged emails with the service team a few times and have a good feeling about their customer support where they helped troubleshoot some problems I faced. They also replaced a faulty part in my kit.

Completeness: “B+”

The kit has a heated glass bed. This will be useful functionality that better kits ought to have; lesser kits on Amazon will lack this. The build plate is of a nice size, giving a 200mm square build service.

The kit is also very Open Source and uses parts one could source as part of the DIY community. That means there is probably a solution for you confusion and ideas on where to go next.

With this kit you should end up with solid foundation for printing PLA, PETG, and ABS. Getting into more exotic materials like wood or carbon reinforced plastics will require minor but accessible and affordable tweaks. With a little effort, and there will be some, this should be a satisfying project.

Parts: mixed “B” and “C”

Electronics. (B) Perfect for a dive into the DIY 3d world. No issue with the arduino clone or the RAMPS 1.4 daughter board. The stepper motor drivers were largely okay but I two nits with those: they could use a little sanding to make them not overlap with each other; second, the potentiometer on those are really finicky (adjustable with a phillips screwdriver) it took me a long time to get those tuned.

Heated bed (C). It works but its also a little saggy. I clipped on all four sides to address this.  I have some trouble heating my bed and current Marlin firmware errors out with it.  My workaround is to heat the bed before doing anything else.

Stepper motors. (B+) I found the same NEMA17 1.8deg motors used elsewhere on machines without too much problem. They work just fine. I would say “A” range motors would be in the 0.9deg range and only slightly more expensive.

Frame is well enough, nothing fancy but put together well enough. Blue (removable) loctite for the large threaded supports iis needed if you don’t want the printer to shake itself apart. (B+)

This hot end has me hot and bothered! (D) My biggest gripe is with the “extruder feeder” - the part that pulls the filament to the hot end. On my kit the spring was far light and as such the filament would not feed properly and my results, esp. on inner fills, show missing lines and impartial fills. RRG support worked with me over the course of a week and helped me get this right. I worry about others may notice the extruder feeder slipping (listen clicking and stalling during prints).

The glass was slightly too big for my build plate once the nuts were added. (B-) I used a dremel and sand small scoops in the chamfered corner sections. This did not take much work but was arguably more danger than I was looking for as a small piece chipped away.

The linear bearings have a bit of grind as much as they have roll. (B) A little grease and the stepper motors don’t seem to mind. I will likely upgrade these.

The chord to the power supply uses the following color codes: yellow, blue, red. (C for danger) The build manual hints at some of these non-standard color codes but I didn’t find a perfect match for this in the guide and I really didn’t want fry the thing.

I used alligator clips and an outlet tester to confirm which is the load, neutral and ground, From what I gather this chord is an old European color code that is no longer standard … but using a US end? It’s weird. This typifies what I think RRG is doing: finding good, but cheap parts, that work with few exceptions. To fill the gap they have a good support team to help customers through the build process.

Documentation: “B”

When I did my build the build manual is version 1.4; configuration manual version 1.1. My notes reference these documents from late August, 2017.

Build Manual: “B”

Bill of Materials incorrect with one of the bags: there’s an amazon review out there that calls this out too. I think it was bag No. 2. There are some large nuts not listed and the counts don’t add up. Don’t worry, march on, even though it annoys me they don’t have correct manual.

The manual covers at least two different version of the kit prior to this one. I noted that in my kit there were hex-shaped bits in some of the molded plastic parts. The manual gets a little confusing where you end up bouncing between following pictures. The manual should be revamped for this generation of the hardware kit.

The manual is generally easy to follow with some few exceptions. Getting the stops correct requires a little thinking. One thing lacking in this manual was how to lay out all the wires. As noted elsewhere the kit comes with just a few zip ties, and no wrapping for the wires. On top of that, how you actually lay these out should be diagrammed somewhere. Mine looks like something I would find buried under the hood in my truck.

Page 17 shows the left and right side panels. I installed my backwards because I was not aware the center frame has a left and right side orientation as well. From the front (fins stick out to the back) the LCD knob hole needs to be on the right side. In my case this just means I’ll print out an LCD display and remount it elsewhere … better for me anyhow.

Configuration Manual: “B”

The configuration manual has some information on setting up Repetier Host and Slic3r. However beyond that you are left guessing which of the config settings you should copy and which you should not. Most of these settings (now that I know better) are decent but this needs more text to explain why they deviate from the defaults.

Post build calibration: “C”

That is … where to go to next?  This is super easy to forget if you know something about 3D printing. I, however, am quite the naif when it comes to this world.  Maybe it's all on YouTube?

Here are some of calibration my prints with [[ASIN:B072LWFXR5 Essentium Engineering Grade PLA]]. I chose this because they are US made, are a top-tier player in the 3d filament world and are involved with developing high end filaments.  I don't know if its much different than general purpose filament PLA such as  [[ASIN:B00ME7CV7C 3D Solutech Real Black 3D Printer PLA Filament]]  I mention because they are different grades.  My blue test print object is from [[ASIN:B00VKSW6PS 3D Solutech See Through Blue PETG]].

I also have my "zombie monkey" print which is exemplifies the stringing and stalling that was happening before I fixed the extruder feed with stronger springs to avoid slipping along the hobbed nut.

Filament: Essentium PLA
Layer Height: 0.2mm
1st Layer Height: 0.35mm  (no more than your nozzle width)
1st Layer Extrusion Width: 175%  (smaller traces 150-175 than default)
1st Layer Speed: 30mm  (keep it slow!)
Bed Temp 1st Layer: 60C
Bed Temp Other Layers: 55C
Extruder Temp 1st Layer: 115C
Extruder Temp Other Layers: 110C
Brims: some

I also have good prints at “208/55C and 202/55C” with this filament.

My calibration print objects:

gingerbread window : thingiverse thing:2633832
gears from (because: gears!) thingiverse thing:2405185
thumb wheel (scaled 0.6) from thingiverse thing:1659528

Last thing to say here: where to go next? thingiverse and tinkercad. At least that’s where I went.

Software: “A”

Slic3r and Repetier-Host are excellent starting places. Prusa also has a version of Slic3r that may be worth using. The RepRapGuru firmware is based on an older version of Marlin.

Service and Support: “B-"

Inconsistent.

With my first service ticket, regarding the hotend filament skipping.  I have a movie of this somewhere.   They answered my email on Saturday, have sent me a replacement part for my extruder feeder along with tracking information. They eyeballed from one of my first test prints that “hey, you have your filament too hot” ... try this.

My next ticket was on the PCB heatbed where I worried that my measured 1.6 Ohm resistance was too high for the heatbed.  They advised me not to use current Marlin firmware.  I had trouble with stall ramp up on heating (I enventually was able to reduce the "bang bang internal" to 1 second to avoid this a little bit).  Then the thermistor wires started to break  RRG advise was for me to zip tie them (I already had t hem zip tied to the bigger wires!) seems they are poorly soldered or too brittle.  Then why sell them to me, people!?

These guys are a US company but that’s not to say the parts are from the US … remember even your phone parts are made overseas.  They shipped my replacement parts for my faulty hot end from somewhere on the East Coast.

