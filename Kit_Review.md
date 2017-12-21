# Kit quality

Worth buying?  Yes.

Here my assessment of the kit, this is my own opinion and yours may differ.

## Overall: "B"

I think its a relatively complete kit with some minor issues.  If you want a frustration-free build experience for a Prusa i3 printer ...  you might want to spend a lot more and get a Prusa i3 kit for many times tthe cost of this kit:  for a clone I am happy at this price point.

- Parts: mixed review, generally the parts are good generic clones.  But everything is a clone.  I did find some issues with my parts that needed revision.
- Completeness: This is a good functional printer, but lacks some of the nicer touches other kits have such as auto-leveling and a good quality filament spool.
- Documentation: Build manual is most of the time easy to follow, but it references older iterations of the hardware which makes things such as the "bill of materials" not quite match up with the current kit.  It also ends abruptly without providing advice on how to get to your first successful print after getting the software installed.
- Software: Open Source and Open Source software.  This is good since the DIY and reprap community is alive and well.
- Service: I have exchanged emails with the service team a few times and have a good feeling about their customer support.

## Completeness: "B+"

The kit has a heated glass bed.  I think a kit has to have at least that functionality to get into Prusa i3 range,
some kits you will find on Amazon will lack this.  The build plate is of a nice size, giving a 200mm square build service.
Again this good.  The kit is also very Open Source which means you have relatively tested and understood parts in the DIY
and 3d printer communities, that means there is probably a solution for you confusion and ideas on where to go next.

With this kit you should end up with solid foundation for printing PLA, PETG, and ABS.  Getting into more exotic materials
like wood or carbon reinforced plastics will require minor but accessible and affordable tweaks.  With a little effort,
and there will be some, this should be a satisfying project.   There are upgrades that this kit does not contain, perhaps
the most popular would be an auto-level sensor, easily enough to add.  The next would be an upgrade to an E3D hotend.

A failing in this kit is its mediocre solution for a filament spool holder.  Prepare yourself to print something up.  The provided pieces of acrylic are designed to hang on a wall mount of some sort.  But really these are not 

## Parts: "B" to "C+"

Grading criteria: a "C" would indicate measurable build quality issues or minimal kit (e.g. no heat bed).
"A" indicates a top-of-the line where we could use the "Prusa Kit" as a baseline.

### Less happy with

This hot end has me hot and bothered!  My biggest gripe is with the "extruder feeder" - the part that pulls the
filament to the hot end.  On my kit the spring was too light and as such the filament would not feed properly and my
results, esp. on inner fills, show missing lines and inpartial fills.  I still have a problem with the gear slipping
with my home-grown spring replacement.  RRG service is sending me a replacement part and I will update with that result.

The borosciliate glass was slightly too big for my build plate once the nuts were added.  I used a dremel and sand
small scoopes in the chamfered corner sections.  This did not take much work but was arguably more danger than I was
looking for as a small piece chipped away.

The linear bearings have as much "grind" as they have roll.  Thankfully the stepper motors are willing to ignore this and I have some lubrication around.  I'll think of them as sliders until I replace them some day.

The chord to the power supply uses the following color codes:  yellow, blue, red.  Even the build manual do not identify which is which.  I used a wall tester, alligator clips and a moment of danger to confirm the assignment. (I describe this in my build notes).  From what I gather, the chord is not US standard but an old European color code.  This typifies what I think RRG is doing: finding good, but cheap parts, that work with few exceptions.  To fill the gap they have a good support team to help customers through the build process.

Kit lacked enough zip ties and didn't have any chord wrap as their pictured unit shows.  So you can't actually build that picture with the nice wrapped chords without purchasing other bits.  This is a minor nit compared to the other parts.

### Happier with

Electronics.  No issue with the arduino clone or its RAMPS 1.4 daugher board.  The stepper motor drivers were largely okay but I have two small complaints with those: first, they could use a little sanding to make them not overlap with each other; second, the potentiometer on those are really finicky (adjustable with a philips screwdriver) it took me a long time to get those tuned.

Frame is well enough, nothing fancy but put together well enough.  I do recommend the blue (removable) loctite for the large threaded supports if you don't want your printer to shake itself apart.

## Documentation: "B-"

I am rather "old school" when it comes to unboxing things.  I like packing slips or bills of materials.  The box came with a single sheet with a pointer to google drive.  The documentation and support files are here:

- [Reprap Guru Prusa i3](https://drive.google.com/open?id=0B4A3jLWIXeoFfkxURVdhMEFpTWpsSExncXFmUGpkalczX3ZvS1J6bGNabGdWM2NwaWNuS0k)

When I did my build the build manual is version 1.4; configuration manual version 1.1.  My notes reference these documents from late August, 2017.

### Spool Holder: "F"

_This is not included in this kit_. What is provided is substandard, in my humble opinion.  It attaches to your wall, I think.  See the picture of mine with a printed hub to center the spool.

### Build Manual: "B-"

Bill of Materials incorrect with one of the bags: there's an amazon review out there that calls this out too.
I think it was bag No. 2.  There are some large nuts not listed and the counts don't add up.  Don't worry, march on, 
even though it annoys me they don't have correct manual.

The manual covers at least two different version of the kit prior to this one. I noted that in my kit there were hex-shaped
bits in some of the molded plastic parts.  The manual gets a little confusing where you end up bouncing between following pictures.  The manual should be revamped for this generation of the hardware kit.

The manual is generally easy to follow with some few exceptions.  Getting the stops correct requires a little thinking.  One
thing lacking in this manual was how to lay out all the wires.  As noted elsewhere the kit comes with just a few zip ties, and no wrapping for the wires.  On top of that, how you actually lay these out should be diagrammed somewhere.  Mine looks like
something I would find buried in my car electronics.

### Configuration Manual: "B-"

The configuration manual has some information on setting up Repetier Host and Slic3r.  However beyond that you are left guessing which of the config settings you should copy and which you should not.  Most of these settings (now that I know better) are decent but this needs more text to explain _why_ they deviate from the defaults.

### Calibration: "F"

Sadly where the kit fails is what to do after setting it up.  Head on over to thingiverse or tinkercad and download some test files.  3DBenchy is a popular calibration print.  I found that a window from a gingerbread house (tall, relatively small, four hard corners) was perfect to dial in the warping and bed adhesion issues.

Right now plan on hitting external documentation, You Tube, and forums on how to dial in the printer to get good prints.  I wish there was a booklet on "getting a good PLA print".  This is hinted at in the Configuration manual as there are settings, but it assumes too much.

## Software: "A-"

Slic3r and Repetier-Host are excellent starting places.  Prusa also has a version of Slic3r that may be worth using.  The RepRapGuru firmware is based on an older version of Marlin.

If you plan on using the current version of Marlin you need the RRG settings copied over.  I have a version of this firmware (ADD POINTER HERE).

##  Service and Support: "A-"

Where I found the parts okay to slightly subpar I also find the service from their support team willing and able to
rectify some of these.  They answered my email on Saturday, have sent me a replacement part for my extruder feeder along with tracking information.  They eyeballed from one of my first test prints that "hey, you have your filament too hot" which wasn't even what I asked.

I did try calling their number which went to voicemail.  But I believe if you do your homework, ask a specific question such as "hey, this doesn't look right" you should be able to engage a good support conversation.

## Reviewer Adjustment: "positive"

Finally, after writing this review.  I think it edges slightly more pessimistic.  If you are DIY'er then go have fun and expect some bumps.  If you are buying this for a 12-year old kid ... prepare to help out.  The 
