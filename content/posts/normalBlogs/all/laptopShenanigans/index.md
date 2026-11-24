---
title: Borrowed exchange laptop shenanigans
date: 2026-11-24
subject: Normal post
topic: All
weight: 10
tags:
  - NixOS
  - Difficulties
summary: Borrowed a laptop for my exchange, it broke and I had to improvize!
---
# What happened?
I wanted to be an exchange student for about a month. Problem being I'm studying programming and didn't have a laptop. The solution was obvious. The school surely has plenty of laptops, right? I was right, I mean it wasn't the best laptop ever but Lenovo Ideapads are known to be fine for sure. Got it a week or 2 before leaving (I do not remember) and thought everything would be fine.

Everything was not fine, 2 ish weeks into the exchange the thing started crashing once every 2 days. Strange. All the errors point to the NVME drive. Probably just some temporary issue, if it gets worse I'll just get some tools and reseat it just in case!

...

...

...

It was not a temporary issue, crashing became more consistent, signs pointed to a physical fault, constant dropping from the bus. Managed a week since staying still helped for the time being. But that didn't last much longer. Managed to make this very website and publish it before it all went to crap.
Can't even boot for 3 minutes, have to improvize.

# The fix(es)
## Check it's not an OS specific thing
Was not, neither Windows or Nix booted, FU-

## Do it the hard way.
Happened to have a pretty sizeable USB stick, around 126 gigs. Had all my ISOs on it through Ventoy. Tried a reinstall of either OS first because why couldn't it be a corrupted drive or something like that? Was not, it kept dropping the drive even in the live environment. At least that's ruled out.

Then it was time to sacrifice the stick. Load the ISO into RAM, partition the stick, install the OS into it, very risky considering I would not have any bootable ISOs after this but we ball. Huh... the wifi dropped? Weird but I can restart it... It worked! A fully booting OS just in the stick without touching the NVME! I fixed it! This is completely fi- 

The wifi... keeps dropping? Why? What? It was fine just a second ago outside of a singular drop, I can't build my actual configs with this????

I mean I can, I just need to constantly restart the driver and the laptop if the driver wouldn't load since Nix keeps finished downloads/build but no sane person would do that... I am not a sane person.

Maybe it was that half-assed config I made just for this to get started? Nope, still broken. Can't do ANYTHING with this. Time to get serious.

## The hardware store.
Found a hardware store open at an odd time on a Sunday, very rare in Italy and extremely lucky for me. Got a hotswappable screwdriver with small Philips heads and a USB cable to get internet through tethering just in case this doesn't work, wasn't that expensive.

## Digging in the insides.
What a pain in the arse this laptop was. Genuinely tough to even get opened and the screws holding the wifi card and nvme down were horrible to screw back in. I eventually managed but I struggled for a solid hour just to reseat some stuff, they did look fine to me at least based on what I saw. Strange.

Aaand the reseat did not help, so now I have to tether for internet AND run the entire thing off a USB stick. Lovely. The best part? The laptop has 3 USB ports. Love it.
