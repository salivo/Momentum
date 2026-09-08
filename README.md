# Momentum
Hand-crafted dual-screen cyberdeck

## Background story:

I wanted to test what it feels like to use Arch Linux on an ARM PC, so the cheapest way for me was to use one of my "toys" (a Linux phone). I went with the Pixel 3a. It used to be my main phone before I drowned it in a river, but I bought a second one (this time not as my main phone, but just for Linux) on a marketplace. I did a basic installation of postmarketOS and realized, hey, this phone is actually pretty usable. Let's try to push its boundaries beyond just being a toy.

I realized I needed a keyboard (I hate gesture controls and the app-centric way phones usually work). I connected a keyboard, set up my main PC configuration, and hey, I even had FreeCAD running on it, which was cool!

It was great, but I wanted to make it genuinely portable. It needed a smaller keyboard attached to it somehow that would be easy to handle. I got the idea to design my own PCB and even started picking out microswitches. Then, I saw another Pixel 3a on the marketplace, and an idea instantly hit me: what if I used another phone as the keyboard? I type on phones a lot, so a touchscreen keyboard is completely fine for me and I'm used to it.

So here we go: a cyberdeck made out of two phones. One acts as an onscreen keyboard that controls the main one via Bluetooth LE, all housed in a custom laptop-style case!

## Features
I needed a laptop or a deck, simply a compute machine, so I don't care about phone calls, cameras, better sleep modes, and the stuff you usually expect from a phone.\
For me, it's not a phone anymore.

Things I like about how it works:
- The keyboard: It looks awesome, feels awesome, is easy to configure, and actually works.
- Automatic suspend: When I suspend the main phone, it suspends the keyboard phone as well.
- Screen brightness control: The keyboard phone's volume controls aren't needed for volume (that's handled by the main phone's buttons), so I use them to control the brightness for both displays instead.
- Weight and build quality: It feels very premium. It's pretty heavy with no cheap plastic feel. Like a high-end Apple-level device or something similar. It's really well assembled, makes no creaking noises, and feels awesome to hold.

What needs to be improved or fixed:
- No OTG support: For me as a hardware hacker and developer, this is an absolute necessity to connect my programmer and see logs via UART or flash chips via JTAG/SWD. If I could do that here, it would be awesome.
- The BLE keyboard takes a while to connect after sleep :( I have no idea how to fix it, but at least it connects reliably every time now.
- The hinges could be built better: The fix is just to use a normal spring, because the current one sucks.

# How it was done

There are three main materials: PLA printed parts, hand-crafted aluminum tubes, and some steel bolts and threaded rod. 

With the printed parts, there was one fun quirk: to print the phone cover, I did a print-in-place :) Where it overhangs, I set an automatic pause, put the phone in there, and let it print directly over the phone. (I'm an engineer, trust me, actually no, I didn't trust myself and was just watching, waiting for it to crack the screen, but it was actually successful!) 

After that, I simply slid the phone out to insert the button caps.

The aluminum pipes were done in a strange way. I wanted to have a thread on the end of each tube, but standard pipes had holes that were too wide, and the bolts would easily fall right into them. So instead, I took a solid rod and used a drill as a makeshift lathe, holding the drill bit with pliers... ahh, it was just messy. Don't try that at home... 

Then there was some weird threaded rod fun. All of this was needed to create a constant-friction hinge, which works pretty well. It's a bit loose, but that's an issue with the spring...

