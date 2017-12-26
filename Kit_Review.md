# Kit quality

Worth buying?  _Maybe!_

If you are relatively confident in tinkering and willing to accept the challenge it can be a rewarding experience. I have learned a lot but I have some issues.

## Overall: "B- / C+"

I think its a relatively complete kit with issues.  If you want a frustration-free build experience this kit contains too many small hazards.

- Parts: I did find some issues with my parts that needed revision.  Most (all) parts a generic ones you will find for DIY kits on 3d forums, etc.
- Completeness: This is a good functional printer, but lacks some of the nicer touches other kits have such as auto-leveling and a good quality filament spool.
- Documentation: Build manual is most of the time easy to follow but it references older iterations of the hardware which makes things such as the "bill of materials" not quite match up with the current kit.  It also ends abruptly without providing advice on how to get to your first successful print after getting the software installed.
- Software: Open Source and Open Source software.  The newer slic3r and (look for the Prusa Slic3r build) are really quite functional.
- Service: I have exchanged emails with the service team a few times and have a good feeling about their customer support where they helped troubleshoot some problems I faced.  They also replaced a faulty part in my kit.

## Completeness: "B+"

With this kit you should end up with solid foundation for printing PLA, PETG, and ABS.  Getting into more exotic materials
like wood or carbon reinforced plastics will require minor but accessible and affordable tweaks.  With a little effort,
and there will be some, this should be a satisfying project. 

A failing in this kit is its mediocre solution for a filament spool holder, does not match the seller description on Amazon.

## Parts: "C"

Let's say a "C" would indicate measurable build quality issues or minimal kit.  On the other end for an "A"  may indicates a top-of-the line where we could use the Prusa branded "Prusa i3" as a baseline.

Things that worked well in my kit

- Electronics:
   - Arduino clone
   - RAMPS board and stepper drivers
   - stepper motors
- Frame, bolts, no missing parts

Things that have troubled me

- The hot end in my kit (a critical component) did not feed properly.  Support helped me out.
- The heated bed on my kit has troubled getting to 100C  (takes fifteen minutes) -- am _working_ with support on this issue.
  PCB droops so I have to clip all four sides.  Resistance on the bed measures 1.6 Ohms which by some accounts is too high 
  for this board. _Finding technical specs on any of these parts is difficult._
- glass plate was a few mm too big for the heatbed ... required using my dremel to bore out corners to fit
- filament spool does not match description at amazon

     {% include image.html url="images/sad_rrg_spool_holder.jpg" description="RRG Spool Holder" %} 

## Documentation: "B"

I am rather "old school" when it comes to unboxing things.  I like packing slips or bills of materials.  The box came with a single sheet with a pointer to google drive.  The documentation and support files are here:

- [Reprap Guru Prusa i3](https://drive.google.com/open?id=0B4A3jLWIXeoFfkxURVdhMEFpTWpsSExncXFmUGpkalczX3ZvS1J6bGNabGdWM2NwaWNuS0k)

When I did my build the build manual is version 1.4; configuration manual version 1.1.  My notes reference these documents from late August, 2017.

### Build Manual: "B"

Bill of Materials incorrect with one of the bags: there's an amazon review out there that calls this out too.
I think it was bag No. 2.  There are some large nuts not listed and the counts don't add up.  Don't worry, march on, 
even though it annoys me they don't have correct manual.

The manual covers at least two different version of the kit prior to this one. I noted that in my kit there were hex-shaped
bits in some of the molded plastic parts.  The manual gets a little confusing where you end up bouncing between following pictures.  The manual should be revamped for this generation of the hardware kit.

The manual is generally easy to follow with some few exceptions.  Getting the stops correct requires a little thinking.  One
thing lacking in this manual was how to lay out all the wires.  As noted elsewhere the kit comes with just a few zip ties, and no wrapping for the wires.  On top of that, how you actually lay these out should be diagrammed somewhere.  Mine looks like
something I would find buried under the hood in my truck.

Page 17 shows the left and right side panels.  I installed my backwards because I was not aware the center frame has a left and right side orientation as well.  From the front (fins stick out to the back) the LCD knob hole needs to be on the right side.  In my case this just means I'll print out an LCD display and remount it elsewhere ... better for me anyhow.

### Configuration Manual: "C"

The configuration manual has some information on setting up Repetier Host and Slic3r.  However beyond that you are left guessing which of the config settings you should copy and which you should not.  Most of these settings (now that I know better) are decent but this needs more text to explain _why_ they deviate from the defaults.

#### Printer calibration: "C"

Where to go to next?  

So here my notes after playing with the build for a week.  Head on over to thingiverse or tinkercad and download some test files.  3DBenchy is a popular calibration print.  I found that a window from a recent gingerbread house design perfect to dial in the warping and bed adhesion issues.

Right now plan on hitting external documentation, You Tube, and forums on how to dial in the printer to get good prints.  I wish there was a booklet on "getting a good PLA print".  This is hinted at in the Configuration manual as there are settings, but it assumes too much.

First: Level your bed properly and set the Z stop.

Second: Budget time to figure out temperature and bed settings.  I burned through about a 0.4kg of filament working through various settings.  Let me share a deviation that I ended up which differs from the "starting place" in the configuraiton manual.

Here are some of calibration my prints with **Essentium PLA**.  I chose this company because they are US made, are a top-tier player in the 3d filament world and are involved with developing high end filamennts.  When it comes to PLA you'll find a few different tiers.  This stuff is good for "functional parts" (like gears) others are also US made but perhaps a different grade of PLA designed for more general use.  This often noticed in the the cheaper $25/1kg vs the $30/.75kg ranges of filament.

 {% include image.html url="images/pla_calibration_print.jpg" description="PLA calibration prints" %} 

- Layer Height: 0.2mm
- 1st Layer Height: 0.35mm **no more than your nozzel width**
- 1st Layer Extrusion Width: 175% **smaller traces 150-175 than default**
- 1st Layer Speed: 30mm  **keep it slow**
- Bed Temp 1st Layer: 60C
- Bed Temp Other Layers: 55C
- Extruder Temp 1st Layer: 115C
- Extruder Temp Other Layers: 110C
- (I find brims are good thing.)

My calibration print objects are:

- gingerbread window : <https://www.thingiverse.com/thing:2633832>
- gears from (because: gears!) <https://www.thingiverse.com/thing:2405185>
- thumb wheel (scaled 0.6) from <https://www.thingiverse.com/thing:1659528>
- 3d benchy (not pictured)

Notes:

- 1st layer height, width, and speed will affecgt how well your plastic "mushes itself into the glass".  You want to see a good buttery print down there.
- Essentium PLA does not like a 30C drop in temp and is not recommended with a bed temp of 70C. I got warping and lifting trying that. Their spec sheet mentions 190-230C but a bed temp max at 60C
- I also have good prints at "208/55C and 202/55C" with this filament.

Last thing to say here:  where to go next?  thingiverse and tinkercad.  At least that's where _I_ went.

Useful links:

- <https://pinshape.com/blog/5-causes-of-a-nozzle-jam-and-how-to-fix-it/> Nozzel Jam
- <https://typeamachines.zendesk.com/hc/en-us/articles/205715759-Making-your-prints-stay-put> Helped me figure out print settings.

## Software: "A"

Slic3r and Repetier-Host are excellent starting places.  Prusa also has a version of Slic3r that may be worth using.  The RepRapGuru firmware is based on an older version of Marlin.

If you plan on using the current version of Marlin you need the RRG settings copied over.  I have a version of the 1.1.6 firmware at <https://github.com/brennane/RRG-Marlin> look at the "example_configuration/RepRapGuru/V2" directory.  But if you like current releases and off-the-shelf this has not, at least, hosed my printer.

##  Service and Support: "A"

Where I found the parts okay to slightly subpar I also find the service from their support team willing and able to
rectify some of these.  They answered my email on Saturday, have sent me a replacement part for my extruder feeder along with tracking information.  They eyeballed from one of my first test prints that "hey, you have your filament too hot".

I did try calling their number which went to voicemail but the VM did mention that email may be best.

I believe if you do your homework, ask a specific question such as "hey, this doesn't look right" you should be able to engage a good support conversation.  Keep in mind that you are engaging a business correspondance so do your half and they'll do theirs.

These guys are a US company.  That's not to say all the parts are from the US ... remember even your phone parts are made overseas.   They shipped my replacement from somewhere on the East Coast.

Good people.

## Reviewer Adjustment: "neutral"

The build manual opens with this expection which I think is appropriate for this kit:

- A little better than basic understanding of electronics
- A little better than basic understanding of mechanical components
- A little better than basic computer skills

This is exactly the sort of kit I would expect at this price point, the number of poor marks I have with having trouble calibrating my machine, it failing my ABS and PET prints on current Marlin give me considerable pause.
