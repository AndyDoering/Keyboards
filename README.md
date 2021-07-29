# The Comprehensive Custom Keyboard Guide

![OldVsNew](https://raw.githubusercontent.com/AndyDoering/Keyboards/main/images/IMG_20191216_164500_596.jpg)

This guide aims to cover everything that you need for leveling up your typing experience. Starting with a brief history, this guide cover components of custom keyboards, how a keyboard works with your operating system, building/modding techniques, the basics of keymap creation and firmware flashing, and finally where to continue exploring and purchasing.

---
## Index:
- [A Brief History](#a-brief-history)
- [Form Factors](#form-factors)
- [Parts of a Custom Keyboard](#parts-of-a-custom-keyboard)
- [How a Keyboard Works](#how-a-keyboard-works)
- [Buying and Building](#buying-and-building)
- [Continue Exploring and Purchasing](#continue-exploring-and-purchasing)

## A Brief History
  This hobby originated from a small niche modding community who wanted more from their boards. Specifically, boards like the Topre switch-based [Happy Hacking Keyboard (HHKB)](https://www.hhkeyboard.com/uk/products/classic/) or the [DK Saver](https://geekhack.org/index.php?PHPSESSID=3eln55ahpfes72egu77cje6s6q0adcv5&topic=44030.0). Most of the knowledge and culture existed on the [Geekhack forum](https://geekhack.org/), where enthusiasts ran limited group buys fulfilled through Google Forms, trust, and PayPal payments. The group buy method, along with communal interest checks on ideas and concepts pre-group buy, still occur largely on Geekhack even today (although more out of tradition than anything). The group buy format remains the most prevalent method for purchasing; however, these usually now occur with full-time online vendors who interface with manufacturers, providing quality-checked consistency, and higher-scale purchase potential. 

  Similar to sneaker culture, getting your hands on some of the kits and other custom keyboard items is a balance of timing, patience, and sometimes a game of packet speed as group buys can sell out in seconds. The limited-run, time-sensitive nature of the buying process has begun to evolve as anti-botting aspects of storefronts are now being implemented to fend off flippers. Fortunately, the components suggested in this article are freely available almost year-round and provide the perfect starting point for someone who is just starting out with this hobby.  

  So now that we have some context, let’s talk about what makes up a custom keyboard. Custom keyboards are considered the gold standard typing experience because of the personal preference and detail they allow. 

## Form Factors
  Form factor refers to the keyboard’s size. Your everyday keyboard is referred to as a full-size (or 100%) and has 104 keys. Tenkeyless (TKL) is a full-size keyboard without the number pad, and typically contains 87 keys. These boards are also referred to as 80% boards. The trend continues with 75%, 60%, 40% and just about every gradation down to 2%, with portions of the board being removed and scaled down as the percentage drops. While these extremely small boards may seem impractical, many enthusiasts use them with a firmware called QMK to map to media and macro keys, use as separate numpads, or to simply flex a collection of hand-crafted artisan keycaps.

  There are also ergonomically (ergo) split boards that separate the board into two boards such as Ergodox, as well as varying layouts such as ortholinear (ortho) seen in 40% boards like the [OLKB Planck](https://olkb.com/collections/planck). Ergodox boards have a devout following as the columnar stagger alignment of keys has become the primary choice for ergonomic use. Ortholinear, which allows for pushing the limits of usability between scale and number of keymap layers, tends to draw a fairly innovative crowd. [This video](https://www.youtube.com/watch?v=bEPg8kk84gw) gives an overview of what it’s like to use an ortholinear keyboard. 

  The main consideration as you increase the board’s size is that you may need more parts, which leads to higher costs. A safe bet is to begin with a 60% size board. Keyboards in this size offer an abundance of mostly plug-and-play parts and can be considered the closest thing to standardized that exists in the community. It is also a cheap place to start and experiment. The case of the board, determined by its form factor, can be plastic, wood, polycarbonate (PC), POM (Polyoxymethylene), brass, stainless steel, or machined aluminum. Higher-end versions of these cases also feature hefty metal weights in the bottom, innovative mounting solutions for the plate and to modify the typing feel, sound, and shock vibrations. Check out this cheat sheet for more information about mounting solutions.

## Parts of a Custom Keyboard
#### Plates
Plates come in a range of sizes, materials, and layouts. The generally accepted takeaways are that metal is a firmer typing experience while softer materials such as PC, POM, FR4 and carbon fiber give progressively more flex (not to mention differing sound profiles). Flex cuts and other design differences are also becoming more commonplace in plate and PCB designs but are omitted from this guide for the sake of brevity. For an in-depth explanation on plate design, see NathanAlphaMan’s interest check post on their [75% Evolv Keyboard](https://geekhack.org/index.php?topic=104531.0).

![PlateTypes](https://raw.githubusercontent.com/AndyDoering/Keyboards/main/images/IMG_20210320_143820_109.jpg)

#### Stabilizers
Stabilizers (AKA stabs) are small pieces of plastic with metal wires that stabilize keys that are larger than 2U or 2 units. Us are the unit of measurement used for keycaps. 1U, the smallest unit possible, is the size of an alpha keycap such as A, B, C, etc. The larger the key, the larger the number before the U in correlation to how many 1U keys it would take up in board space. Without stabilizers, these larger keys would tilt off the switch stems and wind up unusable. Stabilizers come in the more commonly found Costar variants seen in Razer and CoolerMaster boards, or Cherry style. Cherry is the preferred option as they are quieter and smoother than Costar, and can be tuned to a finer degree. Stabilizers also come in PCB or plate mount styles, with PCB mount clipping or screwing into the PCB (with the use of small plastic spacers) and plate mount snapping into cuts in the plate designed for them. The parts recommended in this article are screw-in PCB mounts. For your average 60% board, one 6.25U and four 2U are required.

#### Switches
Now, let’s look at switches. There are literal mega testers that feature 100 or more different switches to try, including a [website by Jacob Alexander of Input Club](https://chart-studio.plotly.com/~haata#/) that illustrates via force curve graphs the amount of force required in a single keypress and release.

There are three main types of switches: linear, tactile, and clicky. The most commonly associated with mechanical keyboards, clicky (Cherry Greens pictured below), generate a click sound via a two-piece stem that taps against the bottom housing of the switch on depress and the bottom of the switch stem on release. The contact on the left is integrated with the pins on the bottom of the switch, and during depress of the switch completes a circuit registering the press as an event. Fast forward through [USB specs](https://www.usb.org/documents) and you’re now seeing letters on the screen as you type.

![MX Green](https://github.com/AndyDoering/Keyboards/blob/main/images/GIF_MXGreen.gif)
	
Tactile switches operate in much the same fashion, but instead of two pieces creating a click noise, the angular shape on the left side of the stem (the moving brown piece in the Cherry diagram below) creates a bump due to resistance in the keypress against the switch leaf. There are varying degrees of ‘bump’ feel, which is dictated by the angle of the stem legs. A more aggressive angle equates to a heavier bump during the keypress. 

![MX Brown](https://github.com/AndyDoering/Keyboards/blob/main/images/GIF_MXRGB_Brown.gif)

Finally, linear switches are those that depress and release in a linear feeling fashion (where the depress and release of a key feels equal in amount of energy required relative to its position in the actuation process), and are often considered the smoothest typing experience. The colors of the switches are commonly used as quick identifiers in brands of what switch type is which since stems cannot be observed in closed housings. Switches, therefore, are described as brand + color. These combinations carry with them a set of statistics such as the Cherry Blacks below: “Linear switching characteristics, 60 cN operating force, 2.0 mm pre travel and 4.0 mm total travel.” See where those force curves from earlier come back into play? Switches are now made with the same number of variables such as housing plastic type, spring type, spring weight (measured in amount of force centi-Newtons (cN) or grams (g) required to actuate the switch), and even preferred types of greases, oils, and gaskets to use on the internal components. All of these boil down to sound-and-feel preferences, and have their own cult followings. #LinearGang. For more switch data, see [ThereminGoats guide](https://www.theremingoat.com/blog/a-beginners-guide-to-force-curves).

![MX Black](https://github.com/AndyDoering/Keyboards/blob/main/images/GIF_MXRGB_Silent-Black.gif)

There are people who chase down vintage boards made in specific regions of the world so that they can harvest well-worn switches from them for the smoothest experience. Sites like [Deskthority](https://deskthority.net/wiki/Main_Page) catalog such information and are an extremely useful resource when hunting vintage West German Cherry Browns and Blacks. Cherry is named for the Cherry Corporation, which was founded in the U.S. in 1953 and began producing keyboards in 1967. The Cherry MX key switch was introduced around 1985, and the MX style ‘+’ shaped stem quickly became the standard switch type to use. Cherry and MX are synonymous from a purchasing perspective, and often advertised as having “Cherry-style” switches. Just know that Alps switches and builds, though, are not for the faint of heart – they are a relic from an older era that are hard to work with, hard to find, and even harder to work on when it comes to your board (That didn't stop me from building [this Lunar AEK](https://github.com/AndyDoering/Lunar-AEK-Build-Log)).

#### Keycaps
TheKeeblog does a stellar walkthrough on each type, but the main factors in keycaps are plastic type, profile, and print method. Plastic options are ABS, PBT, or POM. ABS keycaps are the most basic plastic type, and can be double-shot, pad printed, or laser engraved. ABS also tends to ‘shine’ quicker than PBT, creating a glossy effect on heavily used portions of boards over time. This plastic type was commonly used in older plastic keyboards and gaming consoles and is attributed to the yellowing that occurs over time and with exposure to light (see [RetroBright](https://www.retr0bright.com/) for how to reverse this process). PBT is less prone to shining and yellowing, and is included on boards such as HHKBs, Duckys, Pok3rs, and Realforces. Most of the shelf boards come with OEM profile caps. The tradeoff has been that they are more limited in printing options such as dye-sublimation and only more recently double-shot molding being offered. 


![Keycap Profiles](https://github.com/AndyDoering/Keyboards/blob/main/images/keycap_profiles.png)
- Image by [The Keeblog](https://thekeeblog.com/overview-of-different-keycap-profiles/)
- 
Dye-sublimination is a labor-intensive process that uses a transfer process to create clean crisp marks (legends) on the keycaps. Double-shot uses a mold injection process and two different colors of plastic to create some of the most durable keycaps available and is less prone to showing legends wearing off over time. One last aspect to consider is keycap profile. Keycap profiles, described in rows, are those that can be observed when looking at a keyboard from the side. These change from top to bottom of the board, with each row offering more or less contour to the hand and fingers while typing. The amount of contour naturally requires varying amounts of space and material, and can affect the feel and sound. A web-based tool by reddit user /u/gtderEvan, [Keycaps.info](https://www.keycaps.info/), illustrates these profiles’ names, shapes, and size differences.

No matter what keycaps you buy, make sure you buy the right keys. Normally a base kit is offered with enough keycaps to cover standard (ANSI and Tsangsan) layouts up to TKL size. However, color options, icon keys, and more niche board layouts such as sub 60% sizes, split shifts or spacebars, and ergo boards require the purchase of additional kits to supply the required keys, as seen in the below graphic: 

#### PCBs
The last and often overlooked component, the PCB (printed circuit board), is what makes the keyboard work. It’s the electrical component that links the switches together and allows for actuation signals to be recognized, processed, and delivered to your computer system. PCBs are varying levels of complexity but are normally created with supporting layout styles in mind that range from a fixed variant to supporting the gamut of options in a given form factor (pseudo-affectionately termed Swiss-cheese). PCBs are also often a 1-1 match with the board they are intended to be used with. 60% and some TKL boards  can use interchangeable PCBs, but this is dependent on mounting type of the PCB and stand-off locations in the case. For most everything else, the PCB must be the one sold with the case or kit. Other options include per-key RGB, underboard lighting, ESD protection, USB type (hopefully USB-C), and firmware type (the primary option being QMK).

## How a Keyboard Works
This portion is a more technical walkthrough of how your keyboard works, what QMK offers over everyday keyboard functionality, and what occurs after the keypress. This process begins with plugging in your USB device, which then kicks off more processes. Before you can use a USB device, your system must enumerate the device. The USB port is designed so that inserting (and removing) devices can be recognized by the host. When this happens, the host informs its device driver, which scans the bus and asks the device to identify itself. The question (request) that the host system is making to the PCB is in order to enumerate it, discern exactly what device it is, and how your system should proceed with using it. These descriptors stored in the device describe its capabilities and all the information about it, including the device type (in our case HID), vendor ID, product ID, and more. The device must respond to these calls (along with any other information it may be sending or receiving) with these descriptors in accordance with the specifications found in the report descriptor. This information tells the host system what drivers to use and how to process the information coming in through that USB bus. Once successfully enumerated, the host can begin sending and receiving data (like sending user input to the host system).


![Proton C](https://github.com/AndyDoering/Keyboards/blob/main/images/proton-c.png)
- Image by [u/johananasen](https://www.reddit.com/r/MechanicalKeyboards/comments/aryth0/proton_c_got_the_brains_and_the_looks/)

This process flows like so: device plugged in -> device detected -> get device speed -> get device descriptors -> reset and assign address -> get configurations -> load drivers -> device is ready to use. An example for device descriptors might look something like this:

```c
//------------------------------------------
// Standard Device Descriptor Type Definition
//------------------------------------------
		typedef struct
		{
			BYTE bLength;                // Size of this Descriptor in Bytes
			BYTE bDescriptorType;        // Descriptor Type (=1)
			WORD bcdUSB;                 // USB Spec Release Number in BCD
			BYTE bDeviceClass;           // Device Class Code
			BYTE bDeviceSubClass;        // Device Subclass Code
			BYTE bDeviceProtocol;        // Device Protocol Code
			BYTE bMaxPacketSize0;        // Maximum Packet Size for EP0 
			WORD idVendor;               // Vendor ID 
			WORD idProduct;              // Product ID
			WORD bcdDevice;              // Device Release Number in BCD
			BYTE iManufacturer;          // Index of String Desc for Manufacturer
			BYTE iProduct;               // Index of String Desc for Product
			BYTE iSerialNumber;          // Index of String Desc for SerNo
			BYTE bNumConfigurations;     // Number of possible Configurations
		} device_descriptor;         	 // End of Device Descriptor Type

```

Now that the board is enumerated and ready for use, let’s move on to keypresses. When you press a key, your keyboard is capable of recognizing this as an event (pressed, held, or released). Your keyboard then transfers those presses to the host in the form of a keyboard report containing scan codes, which identifies the board’s current state. The firmware does not send any actual letters or characters, only scan codes. Once the keycode (scan code) is sent to the OS, the software has to match it to an actual character. The HID specification defines what a keyboard can actually send through the USB and be properly recognized. This includes a pre-defined list of scan codes that are simple numbers from 0x00 to 0xE7. An example of this is the scan code ‘0x04’ which correlates to scan code ‘KC_A’, or ‘A.’

Each press is detected through a process called Matrix scanning. This happens approximately 10 times per second. Essentially, what it means is that a keypress is detected as 1 instead of a 0. This process works like a user making a keypress, which is registered by the device firmware. The USB device then sends a bi-directional flow of information over the USB port to the system level data buffer, which is then relayed to the host-side application. If you wanted to modify the codes being sent over the serial bus, then you’d want to use QMK, or the Quantum Mechanical Keyboard. 
QMK is an open source community that maintains QMK Firmware which is based on a fork of tmk_keyboard (by Jun Wako) with some useful features for Atmel AVR controllers. QMK has community adoption and support – from a GUI Configurator to the expansion of a number of available advanced features, and even implementation of the latest trend in firmware flashing, VIA Configurator. QMK should run on any Atmel AVR processor with enough flash memory (the bootlader is default 4kB). The most popular is the atmega32u4, which is an 8-bit AVR RISC-based MCU with 32KB self-programming flash program memory. 

Your keyboard identifies every switch’s state and maps it to a keycode via the help of a C macro, or keyboard layout. Matrix scanning tracks changes since the last scan. QMK stores the last scan, and if different than the current scan, it detects what pressed key caused the difference. The physical switch location corresponds to the Matrix location, which corresponds to the logical switch location linked to the user keymap (which specifies the keycode), or any other user-defined variable, for the logical switch location. These are paired in the keymap.h file, and an example looks like this:

```c
{
		{0,0,0,0},
		{0,0,0,0},
		{0,0,0,0},
		{0,0,0,0},
		{0,0,0,0}
		}
		#define LAYOUT( \
			k00, k01, k02, k03, \
			k10, k11, k12, k13, \
			k20, k21, k22, \
			k30, k31, k32, k33, \
			k40,      k42 \
		) { \
			{ k00, k01, k02, k03, }, \
			{ k10, k11, k12, k13, }, \
			{ k20, k21, k22, KC_NO, }, \
			{ k30, k31, k32, k33, }, \
			{ k40, KC_NO, k42, KC_NO } \
		}

```

The keymap.h file contains the physical mapping of pins and the Matrix definitions for that mapping in two parts. The first part is an ordered array of Matrix positions by switch positions (this maps directly to the keymap). The second is the two-dimensional array that defines the Matrix and pairs it to a Matrix position code. The Matrix scanning loop runs and checks for changes (0 or 1) until a keypress is detected at a defined location (K00). The loop locates [0,0] in the Matrix and finds what key identifier it corresponds to in the layout macro. In the layout, macro K00 will equal a keycode, which is sent to the operating system, or an action is taken such as switching layers, changing lighting, or changing modes such as bootloader or entering debug. The other files are the rules.mk file, which is a make file that is used to set information about the MCU (Microcontroller Unit) that this firmware will be compiled to run on, as well as enabling or disabling some other build features. The config.h file contains the device descriptors such as hardware options, features, and behaviors that were discussed earlier with device enumeration. The file also sets the Matrix size, product name, USB VID/PID, description and other settings, and other defaults to ensure your board is always working.

Finally, the keymap.c file contains the definitions and layermap to keymap data structure. These 16-bit action codes consist of a higher 8 bits, which are all 0 and the lower 8 which holds the USB HID usage code (keycode) such as ‘KC_A’ or ‘0x04’ or ‘00000100’. This is the most often customized and is where the keycodes are stored along with an ASCII art representation of the board layout. All of these files together are used to build the firmware that gets flashed onto the MCU on the PCB –  and then drive all the keypress customization in your keyboard. 


## Buying and Building
Now, we’re ready for the fun part: buying and building. The following list consists of parts commonly chosen for the best budget-friendly custom keyboard. The below picture is close to what your finished board will look like, depending on the keycaps you decide on. 

#### Parts list (prices at time of writing):
```
- Soldering Iron + Tip Cleaner: $48
- Solder: $25
- Desolder Hand Pump: $27
- Flux Pen: $11
- Switch Opener: $10
- Switch Puller: $9
- Keycap Puller: $9
- 60% PLASTIC CASE: $14.90
- DZ60 REV3 60% PCB w/ Case Foam: $48
- DZ60 CNC Plate: $18
- Gateron Yellow (linear) with milky housings 70pcs): $24 
- Stabilizers: $14
- HK Dye-Sub Cherry Profile PBT Keycaps: $39 - $49
- Braided 6 foot USB-C Cable: $12
- GPL105g0 Oil: $10 (OPTIONAL)
- GPL205g0 grease: $10 (OPTIONAL) 

Total Parts and Tools: $310
Total Parts and Tools with Optional Oils and Greases: $330
```

#### The Build Process:

1) [Test PCB](https://www.keyboardtester.com/)
Plugging it into the USB cable on your computer, use tweezers at each switch pin pair on the PCB while the above site is open, which will illuminate the keys on the board and tell you which register correctly and which do not. 
2) [Clip (if needed) grease, and tune stabilizers](https://www.youtube.com/watch?v=usNx1_d0HbQ)
This is an optional component, but it’s often considered an easy and immediate way to improve any board’s typing quality. Clipping the stabilizers removes the unnecessary parts of the bottom of the stabilizer stem where the wire connects in, making the stabilizer less wobbly and unstable. 
3) [Disassemble Switches and Grease Stems and Oil Springs](https://www.youtube.com/watch?v=l8cogVsCmfo)
The other portion of the optional category, and yest again another modification that pays dividends in the typing experience for everything but clicky switches. 
4) Reassemble Switches
5) Install Stabilizers onto PCB
Completed prior to installing anything else, this also affords the opportunity to check how well the stabilizers are tuned by putting in temporary switches and corresponding caps to check the sound and feel of the stabilizer as it makes a full depress and return.
6) Push switches into plate, and into through holes on PCB
7) [Solder Switches to PCB (unless hotswap)](https://youtu.be/iH2mUjJZ-Kw?t=6329)
8) Test PCB again
9) Make any case lining or sound adjustments:
This is a debated area of modding, but generally the cheaper the case, the more it will showcase any sound that occurs during typing. This can be a positive aspect in higher-end cases where sound profile is part of the considerations made in the design and production phases. But in big box or more mass manufactured situations, case lining can lead to a quality heft feeling while managing the echo and vibrations in the case between the bottom of the PCB and inside of the case. 
10) Install solder PCB/Plate/Switch combo into case
11) Put keycaps on
12) Optional flash updated keymaps via [QMK](https://beta.docs.qmk.fm/tutorial/newbs_flashing) or [Via Configurator](https://caniusevia.com/)
PCBs usually come with a default keymap that can be used immediately; however, this is a necessary step if you want to take things a step further (like a function key that switches the arrow cluster to media control keys, or changing lighting options, for example). 
10) Test it out!

[Monkeytype](https://monkeytype.com/) is a stellar customizable typing website that also provides metrics for your progress as you get faster and more accurate. 
Another option you can use for this step is [10 Fast Fingers](https://10fastfingers.com/typing-test/english) as well as [TypeRacer](https://play.typeracer.com/) for racing friends.


## Continue Exploring and Purchasing

A non-exhaustive list of places to purchase the aforementioned components:
- omnitype.com   
- cannonkeys.com
- kbdfans.com
- store.projectkeyboard.com
- novelkeys.xyz
- switchtop.com
- switchmod.net
- olkb.com
- keyhive.xyz
- keeb.io
- spacecat.design
- 1upkeyboards.com
- thekey.company
- originativeco.com

#### Communities for Beginner Keyboard Enthusiasts: 

[![MeetupVideo](https://raw.githubusercontent.com/AndyDoering/Keyboards/main/images/PressESCMeetupVideo.png)](https://www.youtube.com/watch?v=KB6mzNDFcyI "Click to Watch!")

- [Local meetups](https://www.youtube.com/watch?v=KB6mzNDFcyI) are a stellar way to try things out, talk to knowledgable folk, and meet other vendors and makers in the community
- [Top Clack](https://discord.gg/32EgW6N), and [Mechs On Deck](https://discord.gg/m6u3Udw) are all great communities for starting out. Lurking around in the r/mechanicalkeyboards and r/mechmarket subreddits are the most common starting points for people. 
- Twitch is a great place to see [live shows](https://www.twitch.tv/mechsondeck/), [news](https://www.twitch.tv/topclack), and community updates
- Instagram is the best place to get news, group buy updates, follow artisan keymakers.
- Almost everyone has a dedicated Discord server for their vendor site, stream community, etc. This is the best place to interact with other entusiasts and learn more.
- [Deskauthority](https://deskthority.net/wiki/) is an amazing historical and technical resource

![ZachGAFTattoo](https://raw.githubusercontent.com/AndyDoering/Keyboards/main/images/20180915_110449.jpg)
