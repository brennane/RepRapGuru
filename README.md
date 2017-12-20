# Welcome

_Do you have a ReprapGuru or other Prusa i3 clone?_

Here are notes I collected from my build of my "RepRapGuru V2 B" purchased from Amazon during the Fall of 2017.  I believe this is a pretty good kit but will require a little patience and time to understand what's going on, especially from someone rather new to the 3d printing field such as myself.

Should you listen me then?  There's a good question!  All I can say to that end is I've had a colorful and successful field in Computer Science for twenty years.  I am not a _hardware_ guy but I enjoy learning new things, have tackled extremely tough projects over the years, and enjoy hobbies such as _roasting coffee_ and my 3D printer happily sits on an very nice oak side table that I built in woodshop during my school years.  And I live in an older farmhouse which requires a certain amount of upkeep just to keep weatherproofed.  You know, stuff a family man might encounter who has too many kids in a quasi-rural area.

There were things that frustrated me and I quite imagine could baffle someone who is not a programmer or someone who is hobby-minded.  I hope these notes help you overcome similar problems.

A bit on organization:

- Build notes: these describe little notes I made to myself about the build, and some issues I had during the build that are worth noting.
- Initial calibration: after putting the thing together I needed to get a successful print. What to print first?  What settings and filament to use?   There is a lot of conflicting advice out there and I will hopefully cut through some of the noise with sensible settings.  The RRG build manual gets you through initial software setup but lacks information on this important step.
- Firmware: RRG firmware is based on the popular _Marlin_ firmware.  I have an updated branch and hope to commit my "RepRapGuru/V2" configuration upstream.  This isn't necessary but could be useful if you are going to tweak or machine later on.
- Filament: This is a growing list of filament choices I've made and notes I have on "dialing it in" for useful prints.  It is organizing by seller or manfacture and by type.  Here also are configuration notes for the filament for using the filament in a tool such as "slic3r".
- Software: So far I've used a small set of software: "Repetier-Host", "slic3r" and then some toying around on "tinkercad.com" and "thingiverse" for models.

## Kit quality

It is worth mentioning here my assessment of the kit, this is my own opinion and yours may differ.

### Completeness: "B+"

The kit has a heated glass bed.  I think a kit has to have at least that functionality to get into Prusa i3 range, some kits you will find on Amazon will lack this.  The build plate is of a nice size, giving a 200mm square build service.  Again this good.  The kit is also very Open Source which means you have relatively tested and understood parts in the DIY and 3d printer communities, that means there is probably a solution for you confusion and ideas on where to go next.

With this kit you should end up with solid foundation for printing PLA, PETG, and ABS.  Getting into more exotic materials like wood or carbon reinforced plastics will require minor but accessible and affordable tweaks.  With a little effort, and there will be some, this should be a satisfying project.   There are upgrades that this kit does not contain, perhaps the most popular would be an auto-level sensor, easily enough to add.  The next would be an upgrade to an E3D hotend.

### Parts: "B" to "C+"

Grading criteria: a "C" would indicate measurable build quality issues or minimal kit (e.g. no heat bed).  "A" indicates a top-of-the line where we could use the "Prusa Kit" as a baseline.

I give the Kit a "B minus" because I find a good amount of parts that typify a workable Prusa i3 DIY kit that you might find elsewhere on Amazon.  It is not the top-of-line version of these parts which might lead into the "B plus" or "A minus" range.  The nozel is okay but if you were to peek into the firmware you may note that the temperature sensor has this to say about it: `"100k EPCOS - Not as accurate as table 1 (created using a fluke thermocouple) (4.7k pullup)"` compare this prefered thermisters by Semitec which you may choose as an upgrade.  This and other examples lead me to believe the kit is of a servicable quality but allows for upgrades as you grow.

I could argue for a "C plus" for the following two reasons:

1. This hot end has me hot and bothered!  My biggest gripe is with the "extruder feeder" - the part that pulls the filament to the hot end.  On my kit the spring was too light and as such the filament would not feed properly and my results, esp. on inner fills, show missing lines and inpartial fills.  I still have a problem with the gear slipping with my home-grown spring replacement.  RRG service is sending me a replacement part and I will update with that result.
2. The borosciliate glass was slightly too big for my build plate once the nuts were added.  I used a dremel and sand small scoopes in the chamfered corner sections.  This did not take much work but was arguably more danger than I was looking for as a small piece chipped away.

### Documentation: "B"

### Software: "A-"

### Service and Support: "A-"

### Reviewer Adjustment: "positive"

# Notes

## Build Notes

I did the foolish thing: I installed the LCD backwards!  Aye!  I tried to pay attention because this was clearly called out in the build manual but I didn't quite grasp the notion of "front" "back" and whether "right" was "stage right" or "audience right".  In terms of dumb user I think that was the worst of my mistakes and even that one is not fatal.  I simply need to print a part or two and whammo first modification.

This points to my first note on the build: the documentation is pretty good but it requires reading between the lines (or pictures) in some cases.  The manual often refers to older variations of the DYI kit which means some parts will not match or have changed in subtle ways: take your time.  Only a few tools are needed and this should be an enjoyable build.

## Initial Calibration

## _Firmware_

## Filament

## Slicers, Dicers, and Software



----

View this page on [GitHub Pages](https://brennane.github.io/RepRapGuru/)

You can use the [editor on GitHub](https://github.com/brennane/RepRapGuru/edit/master/README.md) to maintain and preview the content for your website in Markdown files.
