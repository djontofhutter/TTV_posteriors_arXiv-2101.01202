# TTV_posteriors_arXiv-2101.01202
Posterior samples of TTV systems in arXix:2101.0120
Description of contents: This repository contains posterior samples for the
    TTV modeling of 48 planetary systems, having 2-4 planets in each system.
    There is one file per planetary system and each file contains five
    columns per planet modeled. There are 10,000 samples per system. 

    The five columns per planet in each posterior sample are as follows:
        mp/Mstar    planet-star mass ratio (in units of MEarth/Msun)
        P           orbital period (days)
        esinω       eccentricity vector (e times the sine of the argument of pericenter)
        ecosω       eccentricity vector (e times the cosine of the argument of pericenter)
        T0          time of the first model transit after epoch BJD-2,455,680.0 (days)

System requirements: The files have no metadata header, and can be read using
    astropy with the command(s):
    
    from astropy.table import Table
    data = Table.read("KOI-1070.dat", format="ascii.no_header")
