---
title: "Ornet-a python toolkit to model the diffuse structure of organelles as social networks"
collection: publications
permalink: /publication/2010-03-18-Ornet-a-python-toolkit-to-model-the-diffuse-structure-of-organelles-as-social-networks
excerpt: 'OrNet is a python framework that models both the spatial and temporal morphology changes that organelles undergo as dynamic social networks.'
date: 2020-03-18
venue: 'Journal of Open Source Software'
paperurl: 'https://doi.org/10.21105/joss.01983'
citation: 'Fazli, M., **Hill, M.** Durden, A., Mattson, R., Loy, A. T., Reaves, B., Courtney, A., Quinn, F. D.,Chennubhotla, C., Shannon Quinn (2020). &quot;Ornet-a python toolkit to model the diffuse structure of organelles as social networks&quot; <i>Journal of Open Source Software</i>. 5(47).'
---

OrNet is a python framework that models both the spatial and temporal morphology changes that organelles undergo as dynamic social networks.

OrNet is an open-source python package (Rossum, 1995) that is built-upon the libraries of
Scikit-Learn (Pedregosa et al., 2011), NumPy (Oliphant, n.d.), SciPy (Virtanen et al., 2019),
and Matplotlib (Hunter, 2007). Our tool accepts as input microscopy videos of cells with
fluorescently tagged organelles, and outputs quantitative descriptions of the morphological
changes. Modeling these dynamic structures is no trivial task because many organelles are
amorphous, and the lack of rigidity renders traditional shape-based, parametric modeling
techniques ineffective. Our framework addresses such difficulities by modeling organelles as
social networks to capture the spatio-temporal relationships via a dynamic edge management
process. The graphs are constructed by fitting gaussian mixture models to every frame of an
input video; the final means become the vertices, while a divergence metric is applied to every
combination pair of mixture components to create the edges. Once graphs are created for
each frame, spectral decomposition is utilized to track the leading eigenvalues to understand
the time-points and frame regions where organellar structures are demonstrating significant
changes.
