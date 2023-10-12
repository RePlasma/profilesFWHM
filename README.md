# profilesFWHM
Cheatsheet for relations between FWHM and W0 or radius for Gaussian profiles

Motivation: for precision simulation modeling of SFQED setups an unambiguous definition of temporal and spatial scales is necessary. Usually experimentalists refer to fwhm in intensity, while for example in PIC codes like OSIRIS the scale is the spotsize in electric field. This notebook provides a quick check on mapping from one definition to the other.

Also includes benchmarking of LG modes in OSIRIS (see input-file photonS.3d)

Notebook by: Óscar Amaro 2023

---


Density: $n=\exp(-0.5x^2/\sigma^2)$
- $\mathrm{FWHM}_n = \sqrt{8 \log 2}~ \sigma$

Gaussian Transverse E-field: $a=\exp(-\rho^2/W_0^2) =\sqrt{I}$
- $\mathrm{FWHM}_a / W_0 = 2\sqrt{\log 2}$
- $\mathrm{FWHM}_I / W_0 =  \sqrt{2 \log 2}$
- $\mathrm{FWHM}_a/\mathrm{FWHM}_I = \sqrt{2}$
