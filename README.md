# PhD thesis — Fire in northern Andean Patagonia

PhD thesis of **Iván Barberá**, Doctor en Biología, Universidad Nacional del
Comahue (CRUB / INIBIOMA), 2025.

**Title (ES):** *El fuego en el norte de la Patagonia Andina: entendiendo sus
controles biofísicos para proyectar el régimen de incendios ante escenarios de
cambio climático.*

**Title (EN):** *Fire in northern Andean Patagonia: understanding its biophysical
controls to project the fire regime under climate-change scenarios.*

Advisors: Thomas Kitzberger (director) and Juan Manuel Morales (co-director).

📄 **[Read the thesis (PDF)](barbera-thesis-2025.pdf)** — 233 pp, in Spanish with
an English summary on the first pages.

## English summary

Northwestern Patagonia is a fire-prone landscape expected to see more fire under
climate change. This thesis studies how physical factors (climate, topography),
vegetation, and human presence control fire across scales, and builds simulation
models to project fire activity under future climate.

- **Site scale.** Paired forest–shrubland comparisons show that the lower
  flammability of forests reflects not only less and less continuous fine fuel
  but also a cooler, moister microclimate that keeps dead-fuel moisture higher.
- **Landscape scale.** All fires over a 24-year period (1999–2022) across
  ~29,000 km² were mapped; burn probability decreases with elevation and
  precipitation, but much of the precipitation effect is mediated by how
  vegetation types of contrasting structure are distributed along the gradient.
  A clear unimodal effect of productivity emerges.
- **Simulation & projection.** A spatially explicit fire-regime simulator of
  three coupled sub-models — **ignition, escape, and spread** — at 30 m / 14-day
  resolution, driven by vegetation, topography, wind, and the Fire Weather Index,
  estimated with hierarchical Bayesian inference (Stan). It was used to project
  burn probability in Nahuel Huapi National Park for the 2040s and 2090s under
  four climate scenarios.

**Keywords:** burn probability, fire-spread models, vegetation, topography,
Bayesian inference, climate change.

## Repository contents

```
barbera-thesis-2025.pdf   Final defended thesis (PDF)
tex/                      LaTeX sources
  main.tex                Master file (document class: report)
  bibliografia.bib        Bibliography (BibTeX)
  apalike-ejor-custom.bst Bibliography style
  configuracion/          Packages and global style (\input by main.tex)
  figuras/                Figures
  secciones/              Chapters and appendices (\include by main.tex)
```

## Building from source

Requires a full TeX distribution (e.g. TeX Live). The bibliography uses BibTeX.

```bash
cd tex
pdflatex main
bibtex   main
pdflatex main
pdflatex main
```

(or simply `latexmk -pdf main.tex`).

## Related work and code

- **Biotic and physical drivers of fire in northwestern Patagonia** — *Fire
  Ecology* (2025). https://doi.org/10.1186/s42408-025-00353-8
- **Microclimate and species composition shape the contribution of fuel moisture
  to positive fire–vegetation feedbacks** — *Agric. & Forest Meteorology* (2023).
  https://doi.org/10.1016/j.agrformet.2022.109289
- **FireSpread** — R package for spatial fire simulation via calibratable
  cellular automata. https://github.com/barberaivan/FireSpread

## Citation

> Barberá, I. (2025). *El fuego en el norte de la Patagonia Andina: entendiendo
> sus controles biofísicos para proyectar el régimen de incendios ante escenarios
> de cambio climático* [PhD thesis]. Universidad Nacional del Comahue.

## License

<!-- >>> Choose a license. Suggested: CC BY 4.0 for the text/PDF, MIT for any code.
     Add a LICENSE file before making the repo public, or state "All rights reserved". -->
To be defined.
