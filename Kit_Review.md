# Kit quality

Worth buying?  A qualified yes.

Buy it if you are relatively confident in tinkering and willing to accept having to figure out whether you are facing a part problem, build problem, or calibration issue.

## Overall: "B" to "B+"

I think its a relatively complete kit with minor issues.  If you want a frustration-free build experience for a Prusa i3 printer ...  you might want to spend a lot more and get a Prusa i3 kit for many times tthe cost of this kit:  for a clone I am happy at this price point.

- Parts: I did find some issues with my parts that needed revision.  Most (all) parts a generic ones you will find for DIY kits on 3d forums, etc.
- Completeness: This is a good functional printer, but lacks some of the nicer touches other kits have such as auto-leveling and a good quality filament spool.
- Documentation: Build manual is most of the time easy to follow, but it references older iterations of the hardware which makes things such as the "bill of materials" not quite match up with the current kit.  It also ends abruptly without providing advice on how to get to your first successful print after getting the software installed.
- Software: Open Source and Open Source software.  The newer slic3r and (look for the Prusa Slic3r build) are really quite functional.
- Service: I have exchanged emails with the service team a few times and have a good feeling about their customer support where they helped troubleshoot some problems I faced.  They also replaced a faulty part in my kit.

## Completeness: "B+"

The kit has a heated glass bed.  This will be useful functionality that better kits ought to have; lesser kits on Amazon will lack this.  The build plate is of a nice size, giving a 200mm square build service.

The kit is also very Open Source and uses parts one could source as part of the DIY community.  That means there is probably a solution for you confusion and ideas on where to go next.

With this kit you should end up with solid foundation for printing PLA, PETG, and ABS.  Getting into more exotic materials
like wood or carbon reinforced plastics will require minor but accessible and affordable tweaks.  With a little effort,
and there will be some, this should be a satisfying project.   There are upgrades that this kit does not contain, perhaps
the most popular would be an auto-level sensor, easily enough to add.  The next would be an upgrade to an E3D hotend.

A failing in this kit is its mediocre solution for a filament spool holder.  Prepare yourself to print something up.  The provided pieces of acrylic are designed to hang on a wall mount of some sort.

## Parts: "B" to "B-"

Let's say a "C" would indicate measurable build quality issues or minimal kit.  On the other end for an "A"  may indicates a top-of-the line where we could use the Prusa branded "Prusa i3" as a baseline.

### Less happy with

This hot end has me hot and bothered!  My biggest gripe is with the "extruder feeder" - the part that pulls the
filament to the hot end.  On my kit the spring was far light and as such the filament would not feed properly and my
results, esp. on inner fills, show missing lines and inpartial fills.  RRG support worked with me over the course of a week and helped me get this right.  I worry about others may notice the extruder feeder slipping (clicking and stalling during prints).

The borosciliate glass was slightly too big for my build plate once the nuts were added.  I used a dremel and sand
small scoopes in the chamfered corner sections.  This did not take much work but was arguably more danger than I was
looking for as a small piece chipped away.

The linear bearings have a bit of grind as much as they have roll.  A little grease and the stepper motors don't seem to mind.  I will likely upgrade these.

The chord to the power supply uses the following color codes:  yellow, blue, red.  The build manual hints at some of these non-standard color codes but I didn't find a match for this.  I used alligator clips and an outlet tester to confirm which is the load, neutral and ground, From what I gather this chord is an old European color code that is no longer standard ... but using a US end?  It's weird.   This typifies what I think RRG is doing: finding good, but cheap parts, that work with few exceptions.  To fill the gap they have a good support team to help customers through the build process.

### Happier with

Electronics.  No issue with the arduino clone or the RAMPS 1.4 daugher board.   The stepper motor drivers were largely okay but I have two small complaints with those: first, they could use a little sanding to make them not overlap with each other; second, the potentiometer on those are really finicky (adjustable with a philips screwdriver) it took me a long time to get those tuned.

Frame is well enough, nothing fancy but put together well enough.  I do recommend the blue (removable) loctite for the large threaded supports if you don't want your printer to shake itself apart.

## Documentation: "B"

I am rather "old school" when it comes to unboxing things.  I like packing slips or bills of materials.  The box came with a single sheet with a pointer to google drive.  The documentation and support files are here:

- [Reprap Guru Prusa i3](https://drive.google.com/open?id=0B4A3jLWIXeoFfkxURVdhMEFpTWpsSExncXFmUGpkalczX3ZvS1J6bGNabGdWM2NwaWNuS0k)

When I did my build the build manual is version 1.4; configuration manual version 1.1.  My notes reference these documents from late August, 2017.

### Spool Holder: "C"

_This is not included in this kit_. What is provided is substandard, in my humble opinion.  It attaches to your wall, I think.  See the picture of mine with a printed hub to center the spool.

 {% include image.html url="images/sad_rrg_spool_holder.jpg" description="RRG Spool Holder" %} 

### Build Manual: "B"

Bill of Materials incorrect with one of the bags: there's an amazon review out there that calls this out too.
I think it was bag No. 2.  There are some large nuts not listed and the counts don't add up.  Don't worry, march on, 
even though it annoys me they don't have correct manual.

The manual covers at least two different version of the kit prior to this one. I noted that in my kit there were hex-shaped
bits in some of the molded plastic parts.  The manual gets a little confusing where you end up bouncing between following pictures.  The manual should be revamped for this generation of the hardware kit.

The manual is generally easy to follow with some few exceptions.  Getting the stops correct requires a little thinking.  One
thing lacking in this manual was how to lay out all the wires.  As noted elsewhere the kit comes with just a few zip ties, and no wrapping for the wires.  On top of that, how you actually lay these out should be diagrammed somewhere.  Mine looks like
something I would find buried in my car electronics.

### Configuration Manual: "B"

The configuration manual has some information on setting up Repetier Host and Slic3r.  However beyond that you are left guessing which of the config settings you should copy and which you should not.  Most of these settings (now that I know better) are decent but this needs more text to explain _why_ they deviate from the defaults.

### Post build calibration: "C+"

That is ... where to go to next.  This is super easy to forget if you know something about 3D printing.  I, however, am quite the naif when it comes to this world.

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

## Software: "A"

Slic3r and Repetier-Host are excellent starting places.  Prusa also has a version of Slic3r that may be worth using.  The RepRapGuru firmware is based on an older version of Marlin.

If you plan on using the current version of Marlin you need the RRG settings copied over.  I have a version of the 1.1.6 firmware at <https://github.com/brennane/RRG-Marlin> look at the "example_configuration/RepRapGuru/V2" directory.  But if you like current releases and off-the-shelf this has not, at least, hosed my printer.

##  Service and Support: "A+"

Where I found the parts okay to slightly subpar I also find the service from their support team willing and able to
rectify some of these.  They answered my email on Saturday, have sent me a replacement part for my extruder feeder along with tracking information.  They eyeballed from one of my first test prints that "hey, you have your filament too hot" which wasn't even what I asked.

I did try calling their number which went to voicemail.  But I believe if you do your homework, ask a specific question such as "hey, this doesn't look right" you should be able to engage a good support conversation.  Keep in mind that you are engaging a business correspondance so do your half and they'll do theirs.

These guys are US.  The company is US, the parts might be from overseas suppliers but that's a different thing; remember even your phone are made overseas.   They shipped my replacement from somewhere on the East Coast.  Good people.

## Reviewer Adjustment: "positive"

Finally, after writing this review.  I think it edges slightly  pessimistic.  If you are DIY'er then go have fun and expect some bumps.  If you are buying this as a christmas present for a family member, be prepared to help out.  The build manual opens with this expection which I think is appropriate for this kit:

- A little better than basic understanding of electronics
- A little better than basic understanding of mechanical components
- A little better than basic computer skills
