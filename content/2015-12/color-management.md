# Notes on color management

~~~
wakeatnight (11:35) about my question yesterday: will printing GIMP-separated CMYK images in Scribus ISO Coated V2 300% result in unstable print?
wakeatnight (12:07) jluc when I printed my photobook with RGB images in Scribus, converted to CMYK PDF via Scirbus and ISO Coated V2 300%, they turned out really bad, no contrast etc. (printer preview showed exactly that too)
wakeatnight (12:08) I tried everything I could and nothing made it better
wakeatnight (12:08) so I separated the images in GIMP and everything looks fine on screen now
wakeatnight (12:08) I am really insecure about all that...
wakeatnight (12:09) so you say the print may turn out OK now (for my quality demands)?
wakeatnight (12:10) quality demands meaning that I don't really know what to expect. They just have to look "OK" with the contrast I wanted when converting RAW to TIFF
wakeatnight (12:10) the printer also suggested using glossy colour paper, even though my images are b&w (but still in RGB space)
jluc (12:11) each change should be color profile managed- whether in scribus or gimp or whatever
wakeatnight (12:11) ah
wakeatnight (12:12) jluc I will print that then (all of my steps are using the ISO Coated V2 300%)
wakeatnight (12:12) have fun and thank you
wakeatnight (12:13) maybe talk to you later?
a-l-e (12:19) just one thing wakeatnight: color management is not about getting better colors, but the expected colors...
wakeatnight (12:19) a-l-e ah yeah. But I wasn't getting "expected colours".
wakeatnight (12:20) It is _really_ complex this whole subject
wakeatnight (12:20) :/
a-l-e (12:20) yep, and the first recipe is: keep it simple :-)
a-l-e (12:21) and the second one: talk to your printer
wakeatnight (12:21) That I did too, hence the recommendations.
a-l-e (12:21) and third: learn gradually...
a-l-e (12:21) step by step
wakeatnight (12:21) So they expect a CMYK PDF so no "Web/Screen" export
wakeatnight (12:22) thank you a-l-e, I try
a-l-e (12:22) starting with a b/w photobook is probably not the best way to build your skills... sadly, this is what you now hat to do :-)
a-l-e (12:24) if possible, now that you got a profile for your monitor (and, i hope, the profiles for the printer), you should create a color managed pdf (target = printer) and ask the print shop for a proof...
a-l-e (12:25) using RGB images is probably easier (since you already have RGB images)... but what counts is that you can compare something on screen and on paper and learn what you can expect from the printer when you see something on your monitor.
wakeatnight (12:29) I see. Using Printer export with RGB images and the right CMYK profiles resulted in a very low contrast print. I do have my display profile.
wakeatnight (12:39) a-l-e what would you recommend, exporting 8 bit TIFFs vs 16 bit TIFFs? Does it even make a difference?
a-l-e (13:05) wakeatnight: i would recommend you not to ask yourself such questions :-)
a-l-e (13:06) now, with the "correct" profile installed and RGB images do you see low contrast images on your monitor?
wakeatnight (13:07) yes
wakeatnight (13:07) sorry
wakeatnight (13:07) no
wakeatnight (13:07) NO
wakeatnight (13:07) it is fine now :)
wakeatnight (13:07) misread your question
a-l-e (13:07) and did you have the correct printer profile installed as you exported the RGB images for printing?
wakeatnight (13:07) yes
a-l-e (13:07) the same as now...
wakeatnight (13:07) ISO Coated V2 300% as recommended by the printer
a-l-e (13:08) so: you're preview on screen is wrong.
wakeatnight (13:08) how do you mean?
wakeatnight (13:08) the screen profile didn't change
wakeatnight (13:08) neither did the printer profile or CMYK
wakeatnight (13:08) the only thing I did that finally yielded nice results on the screen was separating the images in GIMP first...
wakeatnight (13:08) with the same profile!
a-l-e (13:09) color management is not about magic :-)
a-l-e (13:09) as written above: is not about getting good pictures.
a-l-e (13:09) but reliable pictures!
a-l-e (13:09) that means: what you see on the monitor is somehow what you get on paper.
wakeatnight (13:09) well I would need a second test print for that first :)
a-l-e (13:10) i repeat: color management is not about getting contrast rich pictures!
wakeatnight (13:10) but what if I have nice pictures on screen but bad pictures on paper with the correct profiles used?
wakeatnight (13:10) that's not "reliable" isn't it?
a-l-e (13:10) then something is wrong.
wakeatnight (13:10) exactly
wakeatnight (13:10) I would think GIMPs separtion is needed
wakeatnight (13:10) didn't know that before
a-l-e (13:10) no
a-l-e (13:11) it's not needed.
a-l-e (13:11) as said: keep it simple :-)
wakeatnight (13:11) the print result was unacceptable ... :(
wakeatnight (13:11) but why did the Print Preview worked more as expected when I exported in GIMP first?
a-l-e (13:11) i repeat myself: color management is not about getting an acceptable (or not) result back from the printer.
wakeatnight (13:12) I really don't get it.
a-l-e (13:12) it's about getting the same result as you have seen on monitor.
wakeatnight (13:12) yep
wakeatnight (13:12) I wasn't, now the Print Preview suggests I will
a-l-e (13:12) which, at the end, is the only way to reliably get back a good result from the printer...
wakeatnight (13:12) is that bad?
a-l-e (13:12) i have no idea.
a-l-e (13:13) i think that you still did not get what color management is about.
a-l-e (13:13) forget for now, that you want contrast rich pictures.
a-l-e (13:13) what you want, is a good preview on screen of what you get from the printer.
wakeatnight (13:13) OK
a-l-e (13:14) and without getting anything from the printer you cannot check if what you see on screen is correct.
wakeatnight (13:14) that's why I said I want to print the "good result" I have on screen on paper now
wakeatnight (13:14) still no idea why GIMP separation accomplished that
wakeatnight (13:15) maybe RawTherapee is doing something to the images o nexport
a-l-e (13:15) the only test you can now do (without having new proof): if everything is correctly setup, the sames pictures that (it seems) looked ok on monitor correctly but printed without contrast, should now look without contrast on the monitor.
a-l-e (13:15) if this is not the case, you did not setup your color management correctly.
wakeatnight (13:15) I did
wakeatnight (13:15) the Print Preview shoed the same low contrast
wakeatnight (13:15) showed*
a-l-e (13:15) no, not in the print preview.
a-l-e (13:15) the monitor should show them as low contrast.
a-l-e (13:16) at least, this is how i understand color managemnet.
wakeatnight (13:16) so I have to apply the display profile to the whole graphics system?
a-l-e (13:16) color management is about seeing on the monitor what you will get from the printer...
a-l-e (13:16) so: what do you want to apply it to?
wakeatnight (13:16) to the whole window manager?
a-l-e (13:16) no
wakeatnight (13:17) or display output
a-l-e (13:17) scribus will take care of it.
wakeatnight (13:17) I don't know what it's called
a-l-e (13:17) afaik
wakeatnight (13:17) oh wait
wakeatnight (13:17) yes
wakeatnight (13:17) you mean Scribus would show low contrast with Print Preview disabled?
a-l-e (13:17) what the hells is that print preview your talking of?
a-l-e (13:18) keep it simple.
wakeatnight (13:18) Scribus->Colour Management->Simulate Print on Screen
a-l-e (13:18) scribus should show you the same images you used for printing in the same way they were printed.
wakeatnight (13:18) it does
a-l-e (13:18) or close to it.
wakeatnight (13:18) sorry :/
a-l-e (13:19) now, do the same with gimp and install the same color profiles, until you see the pictures in low contrast.
wakeatnight (13:19) I really appreciate you taking time for me but I am really not knowing what to do anymore
a-l-e (13:19) once you've done that, you can start tweaking the images to have contrast!
wakeatnight (13:20) I think I tried and just crushed/clipped the blacks
a-l-e (13:20) (you can also apply the filters in scribus, but i would prefer to do it in gimp)
a-l-e (13:20) converting to CMYK in gimp is (in your case) then useless.
wakeatnight (13:20) OK I have GIMP opened
a-l-e (13:21) ... you don't know enough (nor do i!) about colors to take any profit from an earlier conversion to cmyk.
a-l-e (13:21) just let scribus do it, when creating the pdf.
wakeatnight (13:21) ah
wakeatnight (13:21) so I go to colour management in GIMP now
wakeatnight (13:26) done
wakeatnight (13:26) see the low contrast now
wakeatnight (13:26) colour management + soft proof did that
wakeatnight (13:26) in GIMP
wakeatnight (13:27) adding contrast to it, looks better
wakeatnight (13:27) am checking for clipped blacks
jghali (13:27) for clipped blacks, you should likely enable "black point compensation"
wakeatnight (13:28) did that
wakeatnight (13:28) well looks much better now
wakeatnight (13:30) exporting + checking in Scribus...
jghali (13:32) yep, cmyk cannot reproduce shadows as deep as a screen, so some adaptation is often necessary when converting from RGB to CMYK
jghali (13:32) one of the most common method for that is that "black point compensation"
wakeatnight (13:34) will shadow recovery help?
wakeatnight (13:34) but really, it looks much better now
jghali (13:34) "black point compensation" has an effect only if colorimetric rendering intent is "perceptual", "saturation" or "relative colorimetric"
wakeatnight (13:34) it is set on perceptual
wakeatnight (13:34) (default)
jghali (13:35) this is ok, perceptual is most suited for images
jghali (13:35) have to go, bbl
wakeatnight (13:36) thanks, bye!
Laser87 (13:50) jluc: a-l-e: Now I downloaded the 1.5.1 icon set from github and copied it to /usr/share/scribus/icons - everything fine.
Laser87 (13:50) Archlinux loads it down also, but doesn't copy from temporarily to /usr/share...
Laser87 (13:50) Is this an Arch or Scribus issue?
Laser87 (13:50) I install Scribus-svn with yaourt from the AUR
a-l-e (13:56) have you tried to install with quark? :-)
Laser87 (13:57) I even don't know quark^^
Laser87 (13:58) And I do not use make and install - if it's a problem with the pkg I will report to the maintainer
a-l-e (13:59) i would try to report to the maintainer...
Laser87 (13:59) It's not for me, I'm used to the old icons - I just want to help improving
Laser87 (13:59) Ok, I will contact him
wakeatnight (14:01) a-l-e so I see good results everywhere now on screen using the techniques you recommended...
wakeatnight (14:01) blacks are a bit chrushed but that's fine (and expected, now I know)
wakeatnight (14:01) I guess I go through my pages now and apply this to every image
wakeatnight (14:02) or is there something more that I need to know? I am busy with the stuff I know already :)
a-l-e (14:04) well, you have to know that you won't be sure that it has worked until you got the book back from the press...
wakeatnight (14:04) got it!
wakeatnight (14:04) thanks a lot
a-l-e (14:05) as far i can tell (and i'm really no color expert) the chances are higher that now the book looks better... but you're at your beginnings... and getting a b/w photo book right is probably not really the easiest task...
wakeatnight (14:06) yeah lesson learned I guess
wakeatnight (14:06) but if it prints OK I would be really happy :)
wakeatnight (14:06) one more thing about display profiles. Windows somehow has the profile for my screen - can I copy&paste it into Linux?
wakeatnight (14:06) It's ICM format
wakeatnight (14:07) maybe Ubuntu GNOME has it too though, Ubuntu did, Xubuntu did now
wakeatnight (14:07) did not*
a-l-e (14:28) it does not have to be cross platform... but it might be...
a-l-e (14:28) basically, a wild guess, it depends on your monitor behaving the same on windows and linux... if it's the case, you should be able to copy the profiles...
wakeatnight (14:29) but better to wait and see if Ubuntu GNOME has the profile, too?
wakeatnight (14:29) (maybe the more correct one?)
a-l-e (14:30) again: one question at the time...
a-l-e (14:30) i would try to check if you get reliable colors for now... if it works you can then do more experiments...
wakeatnight (14:30) OK :)
wakeatnight (14:31) so I stick around to Windows then for the time being
~~~
