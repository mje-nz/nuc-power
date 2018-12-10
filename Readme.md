# NUC power supply board
For NUC7i5 and below we've been successfully using the 12V output on the [MATEK UBEC DUO](http://www.mateksys.com/?portfolio=u4a2p).
The included AC power supplies are 19V 65W, and the NUC itself draws about 50W max.
The NUC8i3/5/7 come with a 90W power supply.
The NUC8i5 draws 70W on its own, so the UBEC DUO won't be enough.

This board uses a [DOSA standard](http://www.dosapower.com/) eight-brick power supply module to power a NUC8i5 from a 4-6S LiPo/LiHV battery.
3S batteries will work as long as they start at least half-charged and the voltage is reliably above 9V.
7S and 8S batteries will also work with slightly lower efficiency (70% idle, 85% load vs 80% idle, 93% load), as long as the voltage never spikes over 50V.

It's designed for a [Murata UWE-12/10-Q12NB-C](https://www.digikey.co.nz/product-detail/en/murata-power-solutions-inc/UWE-12-10-Q12NB-C/UWE-12-10-Q12NB-C-ND/5168567) which is a 120W module, but any eighth-brick module will fit (with different performance).
Quarter-brick modules will fit as well, but they'll hang off the edge (and you'd probably get better thermal performance with a bigger PCB anyway).