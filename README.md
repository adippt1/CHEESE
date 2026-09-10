# CHEESE 🧀

**CO<sub>2</sub> Handling & Electrolyzer Engineering Scale-up Evaluator**

CHEESE is an open-source Streamlit dashboard that translates laboratory-scale
CO<sub>2</sub> electrolysis performance into engineering-scale material, flow, energy,
carbon, durability, and screening-level cost requirements. It connects familiar
electrochemical inputs like active area, current density, cell voltage,
Faradaic efficiency, and CO<sub>2</sub> flow, to quantities needed for experimental
planning and scale-up.

CHEESE provides separate **Simple** and **Advanced** interfaces so that new
users can obtain guided estimates while experienced users can access the full
calculation framework.

## What CHEESE can do

### Simple Mode

Simple Mode provides a guided workflow for rapid estimates involving one
primary carbon product and H<sub>2</sub>.

- Predict product formation from electrode area
- Size electrode area from available CO<sub>2</sub> flow
- Calculate CO<sub>2</sub> feed requirements and product-forming utilization
- Calculate total current and direct-current electrical power
- Estimate dry gas outlet flow
- Estimate materials cost per electrolyzer test

### Advanced Mode

Advanced Mode exposes the complete engineering calculation framework.

- Multi-product Faradaic-efficiency distributions
- Gas- and liquid-product production rates
- CO<sub>2</sub> stoichiometry, feed requirements, and utilization
- Reverse electrode-area sizing and stack sizing
- Planning and experimental carbon-balance workflows
- Carbon recovery, recycle, purge, and inorganic-carbon crossover estimates
- Product-specific electricity consumption and LHV/HHV efficiency estimates
- Actual wet-flow interpretation using temperature, humidity, and pressure
- CO<sub>2</sub>-utilization and outlet-composition sensitivity analysis
- Area × stack sensitivity heatmaps and CO<sub>2</sub>-supply constraints
- Carbon-flow Sankey diagrams
- Materials cost per electrolyzer test
- Durability, degradation, downtime, and stack-replacement analysis
- Downloadable CSV result tables

CHEESE includes built-in properties for CO, H<sub>2</sub>, CH<sub>4</sub>, C<sub>2</sub>H<sub>4</sub>, methanol, ethanol,
formate, and methylglyoxal.

## Requirements

A recent Python installation is required. Python 3.11 or 3.12 is recommended
for a fresh installation.

CHEESE directly uses:

- Streamlit
- NumPy
- pandas
- Vega-Altair
- Plotly.py

The required packages are listed in `requirements.txt`. Their corresponding
open-source licenses are summarized in `THIRD_PARTY_LICENSES.md`.

## Getting started

Download or clone this repository and keep the repository files together in
one directory.


## Basic workflow

1. Start in **Simple Mode** for a guided production or sizing calculation.
2. Select the product, Faradaic efficiency, current density, cell voltage, CO<sub>2</sub>
   utilization, and either electrode area or available CO<sub>2</sub> flow.
3. Review the calculated production, current, power, feed, outlet-flow, and
   sizing results.
4. Switch to **Advanced Mode** for multi-product calculations, carbon and
   energy analysis, stack sensitivity, crossover analysis, real-gas
   interpretation, and durability modeling.


## Scope and limitations

CHEESE is an engineering screening and scale-up tool. Its outputs depend on the
operating assumptions and measurements supplied by the user and should not be
interpreted as a complete process design.

The materials-cost module is **not a full techno-economic analysis**. Unless
manually entered, it does not include labor, analytical charges, electricity,
gas procurement, depreciation, maintenance, financing, separations, balance of
plant, or durable test-stand hardware.

Experimental carbon-balance residuals should not automatically be interpreted
as carbonate or bicarbonate crossover. Measurement uncertainty, dissolved
carbon, product crossover, leaks, other carbon losses, and flow/GC
time-alignment should also be considered.

## Citation

A formal CHEESE manuscript citation will be added when available. In the
meantime, use the repository citation metadata in `CITATION.cff`.

## Author

**Aditya Prajapati**  
Lawrence Livermore National Laboratory  
[Read more...](https://people.llnl.gov/prajapati3)

## Getting involved

Questions, calculation checks, bug reports, and feature suggestions are
welcome. Please open a GitHub issue and include the operating assumptions,
inputs, and CHEESE workflow needed to reproduce the behavior.

## Contributing

Contributions may be submitted through GitHub pull requests. All contributions
must be made under the BSD 3-Clause License. See `CONTRIBUTING.md` for the
project workflow and expectations.

## License

CHEESE is distributed under the terms of the BSD 3-Clause License. See
`LICENSE` for details and `NOTICE` for the LLNL auspices and disclaimer
statements.

## Release

CHEESE v1.0  
Copyright (c) 2026, Lawrence Livermore National Security, LLC  
All rights reserved.

SPDX-License-Identifier: BSD-3-Clause  
LLNL-CODE-2023675
