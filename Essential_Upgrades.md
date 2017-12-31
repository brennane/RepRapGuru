#  Extruder Feed (~ $30)

The stock extruder in the kit is non-adjustable.  This a was problem for me since mine was slipping.

I tried to solve the problem by changing out the springs with a heavier set from this $5 box of
compression springs from HomeDepot.  This solved most of the slipping but there was still a fair
amount of slip along the hobbed nut.  The hobbed is the toothy thing that pulls the filament down.
I don't know if the problem is the hobbed nut teeth are too shallow or if the filament guide is too
deep (I think both) but this part was defective.

So they sent me a replacement.  The replacment was pretty nice - heavy springs, a tension control, and
a nice deeply grooved hobbed bolt that grabs the filament.  I don't know it was but it's pretty
close (as far as the filament feed is) to this <http://a.co/a4Pp6Fh>.  Or perhaps this all metal 
one <http://a.co/jheMLYK>.  I price this about $30.

If you were to _just_ get the feeder part you will find the m8 bolts from the kit won't be the correct
length and will have to figure that out.  I'd just get one with the NEMA17 and fan all together.

## Calibration

<https://github.com/brennane/RRG-Marlin> in my "RepRapGuru" example configurations.

### PID tuning

### Extrusion stepper motor feed tuning


# Hotbed change (~ $40)

The hotbed on my kit did not perfom well at all.

So I made the following changes.

1. Swap out the compression springs with heavier ones from my Home-Depot kit from my Extruder fix.
2. Get the Ultrabase plus MK3 kit from Anycubic.  (plus: 220mm bed size) (say around $30)
3. Get an external heatbed controller, I used a BIQU one for about $8.00

## Plumbing

{% include image.html url="http://reprap.org/mediawiki/images/thumb/c/ca/Arduinomega1-4connectors.png/800px-Arduinomega1-4connectors.png" description="RAMPS1.4" %}

1. I connected the D8 pins to the control inputs on the MOS controller.  (The negative line on the MOSFET looks like
long streaks)
2. I connected the heatbed to the MOS controller, and connected the spare powersupply 12V power to this MOS tube as well.

## Firmware and Calibration

I changed the Marlin firmware to use PID temp control for the hotbed.

<https://github.com/brennane/RRG-Marlin> in my "RepRapGuru/V2-Ultrabase"  configurations.

PID tuning:  I changed the defaults to use PID control and the values from my tuning exercise.   I couldn't
find the correct thermistor settings but the ones I have seem pretty close ... close enough.   The following 
logic is applied to this configuration so assumes the same Ultrabase plus BIQU setup I used.

To do your own tuning - in the Repetier-Host G-Code command, issue (from code system):

- `M303 S85 C8 E-1` (tune the heatbed (E-1) to 85C, eight rounds)
- `M304 P313.89 I58.05 D424.30` (apply the results)
- `M500` (save to firmware memory)

# Filament storage (~ $5)

For filament storage I got for *FREE* a frosting bucket from Walmart.  Just ask at the bakery.  Or at H-E-B or Costco.
These tubs are perfectly sized for the filament spools and lock pretty well.  I also have a nice tub from my pool
that used to store chlorine tabs.

I did buy some "orange indicating" dessicant from Amazon, a pound or so, and I just toss a bag of that (with the top opened
up a bit) into the filament tub.

# Filament spool.

The V2 B does not come with a filament spool as pictured.  It has a rather lame couple of pieces of acrylic.  Plan
on printing one of the many available designs from thingiverse.

# Cable chains.

The same goes for cabling protection.  Print or zip-tie.  In my case I found some mesh with the extruder fix and the
new hotbed wires were nicely wrapped in rubber.  As the kit goes, the wiring situation is a mess.
