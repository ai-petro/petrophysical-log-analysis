# Petrophysical Log Analysis

Visual analysis of well log data (Well 15/9-19A, North Sea) using Python and Matplotlib. This project demonstrates standard petrophysical workflows: multi-track log display, statistical distribution analysis, and lithology crossplotting.

## Data

Synthetic well log dataset covering depth interval 3100–3300 m, generated to reflect realistic North Sea formation properties. Logs included:

| Log | Description |
|---|---|
| GR | Gamma Ray (API) |
| CALI | Caliper (in) |
| RHOB | Bulk Density (g/cc) |
| NPHI | Neutron Porosity (v/v) |
| RT | Deep Resistivity (ohm.m) |

## Project Structure

**1. Multi-Track Log Display**
All five logs plotted side by side against depth, replicating a standard log viewer layout (Techlog/Petrel style).

**2. Gamma Ray Distribution**
Histogram of GR values across the interval, used to assess overall lithology (clean sand vs. shale dominance).

**3. Density-Neutron Crossplot**
RHOB vs. NPHI scatter plot, used for lithology identification and porosity trend analysis.

**4. Interpretation**
Written petrophysical conclusion combining all three analyses (see below).

## Key Finding

No confirmed pay zone was identified across the 3100–3115 m interval. Zones of elevated resistivity were found to correlate with tight, low-porosity rock rather than hydrocarbon presence — confirmed by cross-checking RT against RHOB and NPHI, not by relying on RT alone.

**Takeaway:** A single log should never be used to make a formation evaluation decision. High resistivity can result from either hydrocarbons or tight/impermeable rock (e.g. tight carbonate, anhydrite). Distinguishing between the two requires multi-log cross-analysis.

## Tools

Python, Pandas, Matplotlib

## Author

Ali — Petroleum Engineer transitioning into AI/ML for the energy sector.
GitHub: [ai-petro](https://github.com/ai-petro)
