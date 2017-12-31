# Welcome

_Do you have a ReprapGuru or other Prusa i3 clone?_

Here are notes I collected from my build of my "RepRapGuru V2 B" purchased from Amazon during the Fall of 2017.  I believe this is a pretty good kit but will require a little patience and time to understand what's going on, especially from someone rather new to the 3d printing field such as myself.

Should you listen me then?  There's a good question!  All I can say to that end is I've had a colorful and successful field in Computer Science for twenty years.  I am not a _hardware_ guy but I enjoy learning new things, have tackled extremely tough projects over the years, and enjoy hobbies such as _roasting coffee_ and my 3D printer happily sits on an very nice oak side table that I built in woodshop during my school years.  And I live in an older farmhouse which requires a certain amount of upkeep just to keep weatherproofed.  You know, stuff a family man might encounter who has too many kids in a quasi-rural area.

There were things that frustrated me and I quite imagine could baffle someone who is not a programmer or someone who is hobby-minded.  I hope these notes help you overcome similar problems.


# [Kit Review](Kit_Review)


## Would I recommend getting this kit?

I think the answer depends on your ability for DIY projects.  I initially said a _qualified yes_ but
I am having a fair number of issues with my kit.   It's for DIY'ers who can program, use a multi-meter, 
troubleshoot issues, possibly engage forums or support to figure out which end is up.


But the problem I have is with the generic parts, esp. the hot-end and heatbed.  And I had two threads with the support: one very positive that fixed my hotend, and one very disappointing that leads me to believe they know the part is problematic.  Even though it is the cheaper part I had to self-fix (read abandon) the part.

- [My Amazon Review](https://www.amazon.com/review/R2ETPXEMIZBDYI/ref=cm_cr_srp_d_rdp_perm?ie=UTF8&ASIN=B01HOVMLM2)
- [My Kit Review](Kit_Review)

# Build notes

## [Essential (Required) Upgrades](Essential_Upgrades)

I got my kit for about $250 from Amazon, or whatever they were selling them for on Black Friday.  I think a better kit with more fit and finish and fewer part issues is going to cost more ... Anycubic has an attractive kit for $390 over on Amazon.

I solved my major issues with my kit for $40.00 on my end and probably a $20-30 part replacement from RRG support.  Let's call that $70 of "upgrades"  Worth it.  I think for $250 cost yeah.  For something north of $300 ... I am very leery.  Prices and situation changes.

Read details on my [Essential Upgrades](Essential_Upgrades)

## Marlin 1.1.x for RepRapGuru

I have current firmware (Marlin) for this printer that is based on the 1.1.x stable branch.  On github this is [RRG-Marlin](https://github.com/brennane/RRG-Marlin) note the default branch is called "1.1.x-RRG-Amazon" and I have example configs for the stock "V2 printer" and the one with my essential upgrades in "V2-UltraBase".

These you may find useful.  No warranty expressed or implied.

# Initial calibration

After putting the thing together I needed to get a successful print. What to print first?  What settings and filament to use?  There is a lot of conflicting advice out there and I will hopefully cut through some of the noise with sensible settings.  The RRG build manual gets you through initial software setup but lacks information on this important step.

# Firmware: 

RRG firmware is based on the popular _Marlin_ firmware.  I have an updated branch and hope to commit my "RepRapGuru/V2" configuration upstream.  This isn't necessary but could be useful if you are going to tweak or machine later on.

# Filament

This is a growing list of filament choices I've made and notes I have on "dialing it in" for useful prints.  It is organizing by seller or manfacture and by type.  Here also are configuration notes for the filament for using the filament in a tool such as "slic3r".


----

View this page on [GitHub Pages](https://brennane.github.io/RepRapGuru/)

You can use the [editor on GitHub](https://github.com/brennane/RepRapGuru/edit/master/README.md) to maintain and preview the content for your website in Markdown files.
