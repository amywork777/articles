# Adhesives are the invisible discipline holding your product together

If you take apart a modern phone, a pair of headphones, or an EV battery pack, you'll find fewer screws than you'd expect and a lot more glue. Adhesives are quietly replacing fasteners across nearly every category of physical product, and the engineering discipline behind them is one of the least understood in the industry.

"Use glue" is not a spec. The wrong adhesive, applied wrong, will turn into delamination or sudden bond failure six months after the product ships. The right one will outlive the rest of the product. The difference comes down to chemistry and process knowledge that mostly lives in the heads of a few hundred application engineers worldwide.

The first thing you have to understand is the split between thermosets and thermoplastics.

## Thermosets vs thermoplastics

Adhesives fall into one of two camps based on how they cure.

**Thermosets** cure by chemical reaction. The molecules form irreversible bonds with each other and build a rigid network. Once cured, they don't melt. They don't reflow. They are what they are forever. Epoxies and super glue are thermosets. They're strong, temperature-stable, and unforgiving.

**Thermoplastics** cure by phase change. They melt, flow into the joint, and re-solidify on cooling. Apply heat again and they melt again. Hot melts and pressure-sensitive tape adhesives are thermoplastics. They're fast to apply, forgiving, and easy to automate. They're also softer and creep over time.

The choice between them is the most consequential decision in the bond design.

A good rule of thumb: if it has to survive a hot car in Phoenix in August, you want a thermoset. If it has to come off the assembly line every four seconds, you want a thermoplastic.

## How they fail

Both fail, just differently.

Thermosets fail brittle. They reach their ultimate strength and shatter. The first sign of failure is a part on the floor.

Thermoplastics fail by creep. Under sustained load, they slowly flow over months or years. The geometry shifts, the joint loses preload. You can see this coming if you instrument for it. You almost never do.

This is why a properly cured thermoplastic with conservative numbers will sometimes outlast a thermoset with much higher rated strength.

## Where bonds actually fail

Two things kill more bonds than the adhesive itself: surface prep and joint geometry.

The strongest adhesive in the world cannot bond to a contaminated surface. Mold release, fingerprints, dust, oils that migrate out of nearby plastics over time - any of these will give you a beautiful-looking bond that pops apart at the first thermal cycle. A good adhesive engineer spends more time thinking about surface prep than about which adhesive to pick.

Joint geometry is the other one. Adhesive bonds are dramatically stronger in shear (the substrates trying to slide past each other) than in peel (one substrate trying to lift off at an edge). The ratio is often ten to one or worse. Almost every catastrophic adhesive failure I've seen has been a peel failure on a joint the designer thought was loaded in shear.

The other quiet killer is thermal expansion. Two materials with different coefficients of expansion will fight each other through the bondline every time the temperature changes. A part that passes static load tests on day one starts coming back from cold-climate customers six months later, because the bond couldn't survive a hundred trips between -20°C and +25°C.

## Why this matters now

Adhesives are eating fasteners everywhere. Apple uses adhesive instead of screws in nearly every assembly. EV battery packs are bonded into structural members. Aerospace composites are entirely adhesive-bonded; bolts would defeat the point of using composites at all.

But the design tooling has not kept up. The state of the art is still a PDF data sheet and a phone call to the vendor's tech rep. There is no good simulation. There is no integration in mainstream CAD that lets you specify, simulate, and verify a bonded joint the way you can a bolted one.

A discipline that quietly underwrites a huge fraction of the products you use every day, run by a small community of specialists, with almost no good software. If you're an engineer looking for somewhere with depth and very little public knowledge, this is one of the best places to look.

---

## Further reading

- *Adhesion and Adhesives Technology* by Pocius - the standard textbook
- 3M technical bulletins on adhesives (free, surprisingly good)
- Henkel Loctite design guides
- Kinloch's *Adhesion and Adhesives* for the surface science fundamentals
