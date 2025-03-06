```mermaid
graph TD;

subgraph In_Progress
  id3["Cherry MX, Kailh Choc V1"] --> id4["Redragon Low Profile (reversible)"];
  id5["First prototype is under production"];
end

subgraph To_Do
  id1["Laser cut switch-bottom plates (minimalist, full plate, etc)"];
  id2["my own ZMK firmware"]
  id3["MX, Kailh Choc V1, Redragon switch support"]
end


```
- Kicad 9.0 or newer maybe required
- This project aims to change only the switch being used while minimizing changes to everything else to maintain the best compatibility.
- This is my first time using KiCad. May you and the Lord forgive me if files contain any mistakes or issues (It's the reason why I remove the support for both MX and Choc V1, I wasn't sure if I can make it work).
- [Redragon Low Profile footprint]( https://github.com/rgoulter/keyboard-labs/blob/master/pcb/ProjectLocal.pretty/SW_Redragon_LowProfile_PCB_1.00u.kicad_mod
) is from  [Rgoulter](https://github.com/rgoulter). Kudos to this man.

<img src="./images/complete layers original.png" alt="complete layers original" width="700"/>
Original PCB
<img src="./images/complete layers redragon.png" alt="complete layers red dragon" width="700"/>
Redragon PCB
<img src="./images/What will multi switch support looks like.png" alt="for blind people, I just put redragon footprint on top of the old design" width="700"/>
If I just put redragon footprint on top of the old design, I think this will work with minimal change to the number 2 pad (make it smaller ?) I will try, 2$ per order anyway.
<img src="./images/MX_Redragon_Choc.png" width="700"/>
The tri-switch-supported version (MX, Redragon, Choc) will have different stem hole cutouts, with MX and Choc featuring larger openings than Redragon. To prevent short circuits, Redragon switch pins have to be bent when installed.
<img src="./images/FirstPrototype.png" width="700"/>
First Protorype I ordered on JLCPCB


# cheapis (The Original)

v0.1 issues:
- most ubs cables cannot be plugged in when the pro micro is soldered in an usual way (upright, with the usually included pins), because of the top middle buttons. It has to be solderes upside down, flush with the keyboard pcb.
- not really an issue, but SOD-323 diodes are challenging to solder. They're also not the cheapest, although the difference is minuscule.

Cheapis was inspired by ferris and sweep.

It is the cheapest alternative to the above keyboards (that still has a PCB) as it is sub 100x100mm in size so it can be ordered for a very low price and it only needs one controller (Pro Micro or alternative).

![cheapis keyboard!](/cheapis_v0.1_built.jpg "cheapis keyboard built")

![cheapis keyboard!](/cheapis_v0.1.jpg "cheapis keyboard")

Specs:
- Split
- Unibody
- 34 key
- Compatible with MX, Kailh Choc v1 and Gateron low profile switches
- needs 1n4148 SOD-323 diodes
- 19mm standard spacing
- angled sides by 20 degree

Pros:
- less than 100x100mm
- reversible, so you can order less
- needs ony one Pro Micro or alternative
- very cheap way to experiment with 34 key layout

Cons:
- it has to be unibody
- tenting is not possible
- fragile without a plate as the Pro Micro keeps the two sides together
- not much features, it's hardly more than a hardwire
