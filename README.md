# Portable RJ45-to-Eurorack Bridge

## A system that allows impromptu collaboration between Eurorack modular synthesists, while maintaining an appropriate distance during the COVID-19 pandemic.

This is essentially a breakout for a shielded RJ45 jack. Each of the 8 pins of the RJ45 jack is connected to the tip of a 3.5mm jack (the Eurorack standard for patch cables). Connecting a *shielded* Ethernet cable between two of these essentially allows eight CV or audio signals to reach across a long distance, from one modular synth to another.

### Ideas

* You and your collaborator each build one of these, then meet up and create sound together, while maintaining a safe distance.
* Or make two (Oshpark gives you 3 boards anyway!) and keep them with your modular travel case for impromptu collaborations.
* Consider working/performing outdoors, over a fence, from neighboring houses, or in separate cars.
* Indoors, try collaborating blindly while in separate rooms without telling each other what kind of signal is on each of the jacks. Change them mid-performance.
* Labeling the jacks isn't so useful if your partner labels them differently. That fine though - that might force experimentation, chance, and fortunate mishaps.
* Come up with some kind of system of rules that provides structure for chance happenings: the left four jacks are for inputs, the right are for outputs; or one person sends gates or envelopes through the left jacks and the other person returns audio on the opposite jacks. (Accidentally connecting an output to an output generally isn't a problem in Eurorack - nothing should blow up.)
* Think about collaboration in terms of live performance or as two different recordings to be made simulataneously by each of the collaborators.
* Come up with a more unidirectional scenario: maybe one person supplies a different looping sample on each of the eight jacks and the other must use them in their composition. Then switch roles at some point.
* Use a cable that will provide you the CDC-recommended social distance. Maybe see what happens with an extremely long cable combined with a very loud PA at both ends. Or a Twitch live stream from both ends. Or a phone call?

![Two Units with Yellow Cable and Aluminum Enclosure](/photos/two_units_with_yellow_cable.jpg)

### Build

1. Make the circuitboard using the files provided (or buy it from https://oshpark.com/shared_projects/3NctJJYb)
2. Solder the required components
  * 1 x Wurth Elecktronik Shielded Ethernet Connector p/n 615008140421 from [Mouser](https://www.mouser.com/ProductDetail/Wurth-Elektronik/615008140421?qs=%2Fha2pyFadujj32eJSvwd90ECqRKXOEYbwVGH%2FNq2N1eMDIxBQFOhvg%3D%3D)
  * 8 x PJ301M-12 3.5mm switching mono jacks (aka Thonkiconn) from [Thonk](https://www.thonk.co.uk/shop/3-5mm-jacks/), [AI Synthesis](https://aisynthesis.com/product/3-5mm-eurorack-jack-thonk-pj301m-12/), [Control](https://www.ctrl-mod.com/products/3-5mm-eurorack-jacks), [synthCube](https://synthcube.com/cart/3-5mm-euro-jacks), etc
3. Make an enclosure using the template provided or purchase a Hammond Manufacturing 1590A diecast aluminum enclosure p/n 1590A from [Mouser](https://www.mouser.com/ProductDetail/Hammond-Manufacturing/1590A?qs=lxPAlgZqN%2Fx6Rw4O%2FIXFww%3D%3D)
4. Get a hold of a *shielded* ethernet cable  

### Build Tips

* Remember that Oshpark gives you 3 PCBs when you order!
* If you use a different PCB fab service, make sure the castellated holes aren't going to be a problem (ie: they should to be plated)
* When soldering the jacks on, it's easiest if you bend in the pin that connects to the castellated hole before inserting it into the pcb. Heat the pin from the outside and apply solder at the point where the castellated hole is.
* Consider soldering the 3.5mm jacks on first, then the ethernet jack. Otherwise, it won't sit flat on the table when you try to solder the 3.mm jacks.
* You'll need to make a rectangular hole in the enclosure for the ethernet jack. If you're using a diecast aluminum enclosure, it's easiest to do this with a milling machine but you can also drill a hole and carefully turn it into a rectangle using a triangular file.

### FAQ

- **Haven't I seen this before?**
  - Other patch cable bridges/busses definitely exist, although I've only seen them as modules or integrated into a case. The idea with this one is that it's portable, shareable, and doesn't take up real estate in the case when you're not collaborating. With that said, you can of course use it to connect two of your own cases, as you would with a module like Intellijel's Octalink, the Doepfer A-180-9, or the ADDAC213 Eurorack Bridge.

- **Can I connect this to an ethernet hub/switch or a computer?**
  - Don't do that. Don't connect the other end of the ethernet cable to anything other than another one of these devices. You could probably connect it to one of the modules listed in the previous FAQ but I haven't tried it.

- **Can I make these and sell them?**
  - The [GPL license](https://github.com/rahji/rj45eurorackbridge/blob/master/LICENSE) allows you to do this, with certain conditions. This is meant to be an inexpensive DIY project, not an overpriced product for you to sell at a 300% markup on Tindie. No matter what, please don't remove the Black Lives Matter silkscreen (see below).

- **Why does the PCB say Black Lives Matter?**
  - Because it's an important message to have anywhere and everywhere. (More info to follow on this one.)

![Two PCBs, After Soldering](/photos/two_units_after_soldering.jpg)
![Two PCBs, Front and Back](/photos/pcb_back_and_front.jpg)

