# OceanEmbed Prototype

Prototype for reconstructing North Indian Ocean subsurface temperature from surface ocean observations using a Fourier Neural Operator (FNO).

## Project Overview

OceanEmbed aims to reconstruct subsurface ocean temperature from surface-observable ocean variables.

The current prototype uses data from the Copernicus Marine Service, specifically the GLORYS12V1 global ocean physics reanalysis.

The planned model takes surface ocean fields as input:

- Sea Surface Temperature (SST)
- Sea Surface Salinity (SSS)
- Sea Surface Height (SSH)

and predicts ocean temperature at multiple depths.

The overall learning problem is:

```text
Surface Ocean Fields
        │
        ├── SST
        ├── SSS
        └── SSH
        │
        ▼
   Fourier Neural
      Operator
        │
        ▼
Subsurface Temperature
at Multiple Depths
