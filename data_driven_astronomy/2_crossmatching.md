# Cross-matching

When investigating astronomical objects, like active galactic nuclei (AGN), astronomers compare data about those objects from different telescopes at different wavelengths.

This requires positional cross-matching to find the closest counterpart within a given radius on the sky.

In this activity you'll cross-match two catalogues: one from a radio survey, the [AT20G Bright Source Sample (BSS) catalogue](http://cdsarc.u-strasbg.fr/viz-bin/Cat?J/MNRAS/384/775) and one from an optical survey, the [SuperCOSMOS all-sky galaxy catalogue](http://ssa.roe.ac.uk/allSky).

The BSS catalogue lists the brightest sources from the AT20G radio survey while the SuperCOSMOS catalogue lists galaxies observed by visible light surveys.
If we can find an optical match for our radio source, we are one step closer to working out what kind of object it is, e.g. a galaxy in the local Universe or a distant quasar.

We've chosen one small catalogue (BSS has only 320 objects) and one large one (SuperCOSMOS has about 240 million) to demonstrate the issues you can encounter when implementing cross-matching algorithms.

![image](https://groklearning-cdn.com/modules/5JAX7dX9j4wdXKXRHwyECd/Ra_and_dec_demo.gif)

The positions of stars, galaxies and other astronomical objects are usually recorded in either equatorial or Galactic coordinates.

Equatorial coordinates are fixed relative to the celestial sphere, so the positions are independent of when or where the observations took place.
They are defined relative to the celestial equator (which is in the same plane as the Earth's equator) and the ecliptic (the path the sun traces throughout the year).

A point on the celestial sphere is given by two coordinates:

**Right ascension**: the angle from the vernal equinox to the point, going east along the celestial equator;

**Declination**: the angle from the celestial equator to the point, going north (negative values indicate going south).

The vernal equinox is the intersection of the celestial equator and the ecliptic where the ecliptic rises above the celestial equator going further east.

The coordinates of stars in the sky will change slightly over the years due to the slow wobble of Earth's axis.
Therefore, it is important to specify the epoch or time period which we are using as a reference for the celestial coordinate system.
