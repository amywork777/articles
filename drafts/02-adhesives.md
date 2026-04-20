# Adhesives are the invisible discipline holding your product together

If you take apart a modern consumer product (a phone, a pair of headphones, a laptop, an EV battery pack) you'll find fewer screws than you expect and a lot more glue. Adhesives are quietly replacing fasteners across every category of physical product, and the engineering discipline behind them is one of the least understood in the industry.

"Use glue" is not a spec. The wrong adhesive, applied wrong, will turn into delamination, creep, or sudden bond failure six months after the product ships. The right adhesive, applied right, will outlive the rest of the product. The difference between those two outcomes comes down to a body of chemistry and process knowledge that mostly lives in the heads of a few hundred application engineers worldwide.

This is the introduction. The fundamental split you have to understand first is thermosets versus thermoplastics.

## Thermosets vs thermoplastics

Adhesives, like all polymers, fall into one of two camps based on how they cure.

**Thermosets** cure by chemical cross-linking. The molecules form irreversible covalent bonds with each other during cure, building a rigid three-dimensional network. Once cured, they do not melt. They do not re-flow. They are what they are forever. Epoxies, polyurethanes, cyanoacrylates (super glue), and most structural adhesives are thermosets.

Thermosets are strong, temperature-stable, and chemically resistant. They are also brittle, slow to cure, and unforgiving of bad surface prep.

**Thermoplastics** cure by physical phase change. They melt above some temperature, flow into the joint, and re-solidify on cooling. Apply heat again and they melt again. Hot melts (EVA, polyamide, polyolefin) and pressure-sensitive adhesives (PSAs - the stuff on tape and labels) are thermoplastics.

Thermoplastics are fast to apply, forgiving of contamination, repositionable, and easy to automate. They are also softer, lower in temperature ceiling, and prone to creep under sustained load.

The choice between them is the most consequential decision in the bond design.

## When to use which

Thermosets win when you need:
- Structural strength (load-bearing joints)
- High temperature resistance (anything that sees over 80°C in service)
- Chemical resistance (solvents, fuels, automotive fluids)
- Long-term dimensional stability
- A bond that will see many years of thermal cycling

Thermoplastics win when you need:
- Fast assembly cycle times (seconds, not minutes or hours)
- Repositioning before final cure
- Bonding to dissimilar substrates with high CTE mismatch (the compliance helps)
- Softgoods lamination (where the substrates themselves are flexible)
- Easy disassembly for repair or recycling

A good rule of thumb: if it has to survive a hot car in Phoenix in August, you want a thermoset. If it has to come off the line every four seconds, you want a thermoplastic.

## How they fail

Both fail, just differently.

Thermosets fail brittle. They reach their ultimate strength and shatter. The bondline cracks, propagates, and the joint comes apart catastrophically. You will not get a warning. The first sign of failure is a part on the floor.

Thermoplastics fail by creep. Under sustained load, they slowly flow over hours, days, or years. The bondline thins, the geometry shifts, the joint loses preload. You can see this coming if you instrument for it. You almost never do.

This means cure chemistry matters more than the data sheet strength number. A thermoset rated to 5000 psi shear that's been improperly cured (wrong ratio, wrong temperature, wrong time) might give you 1500 psi in practice and fail brittle the day after warranty expires. A thermoplastic with conservative shear numbers might quietly outlast every other component in the assembly.

## Surface prep

This is where most adhesive bonds actually fail.

The strongest adhesive in the world cannot bond to a contaminated surface. Mold release, fingerprints, dust, oxide layers, plasticizer migration from nearby parts - any of these will give you a beautiful-looking bond that pops apart at the first thermal cycle.

Two material families are particularly hostile: silicones (used in seals, potting, and a lot of medical/automotive applications) and fluoropolymers like PTFE (Teflon). Both have surface energies so low that nothing wets them. To bond to silicone or PTFE, you have to physically or chemically modify the surface first.

The three main surface treatment options:

**Plasma treatment** uses ionized gas to clean the surface and add reactive sites. Atmospheric plasma is fast and dry-line-compatible. Vacuum plasma is more aggressive but requires a chamber.

**Corona treatment** is the cheap continuous-process version of plasma. Most film and web converting lines run corona inline. Less aggressive than plasma but enormously cost-effective at volume.

**Chemical etch** uses acids or sodium-based etchants to physically roughen and chemically modify the surface. Aggressive, dirty, regulated, and sometimes the only thing that works for fluoropolymers.

A good adhesive engineer will spend more time on surface prep than on adhesive selection. The adhesive vendor's technical rep will tell you this on the phone, but it never makes it into the data sheet.

## Bondline geometry

The other place bonds fail is the joint design.

Adhesive bonds are dramatically stronger in shear than in peel. A bondline that's loaded in shear (the two substrates trying to slide past each other) can be ten or a hundred times stronger than the same bondline loaded in peel (one substrate trying to lift off the other at one edge).

Almost every catastrophic adhesive failure I've seen has been a peel failure on a joint that the designer thought was loaded in shear. This usually happens because the load path was misjudged, or because thermal expansion induced a peel component that wasn't in the static analysis.

Some hard-won design rules:

- Always design for shear loading, never peel
- Bondline thickness has an optimum, usually around 0.005-0.015 inches; thicker is not stronger
- Lap joint length has a limit too; past a certain length, the additional area carries no load (stress concentrates at the ends)
- Match the moduli of your substrates and adhesive as closely as you can
- CTE mismatch will tear bonds apart over thermal cycles even when the static strength is fine

The CTE mismatch one bites everyone the first time. You build a part that passes static load tests, ship it, and start getting field returns six months in from customers in cold climates. The bond was strong enough on day one. It just couldn't survive a hundred trips between -20°C and +25°C.

## Why this matters now

Adhesives are eating fasteners across the industry. Apple uses adhesive instead of screws in nearly every assembly. EV battery packs are bonded into structural members. Aerospace composites are entirely adhesive-bonded - bolts would defeat the point of using composites at all.

But the design tooling for adhesives has not kept up. The state of the art is still a PDF data sheet and a phone call to the vendor's tech rep. There is no equivalent of FEA for bondlines that gives you reliable answers. There is no integration in mainstream CAD that lets you specify, simulate, and verify a bonded joint the way you can a bolted one.

This is a discipline that quietly underwrites a huge fraction of the products you use every day, run by a small community of specialists, with almost no good software. If you are a tools-builder looking for an underserved market, or an engineer looking for a discipline with depth and almost no public knowledge base, adhesives are right there.

---

## Further reading

- *Adhesion and Adhesives Technology* by Pocius - the standard textbook, dense but worth it
- *The Mechanics of Adhesion* edited by Dillard and Pocius - if you want the math
- 3M technical bulletins on PSAs and structural adhesives (free, surprisingly good)
- Henkel Loctite design guides for threadlockers and structural adhesives
- ASTM D1002, D3163, D3433 - standard test methods for lap shear and fracture
- Kinloch's *Adhesion and Adhesives* for the surface science fundamentals
