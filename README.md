# Lineage-Tree-Analysis
Visualized cell lineage trees from tracking data and analyzed cell division patterns.

# Steps Performed
1. Loaded lineage data from CSV file
    - Import Libraries
    - Load Data
2. Created tree diagrams to visualize top 5 largest lineages with color-coded morphology.
    - Identify Root Cells (no parent)
    - Build Parent-Child Relationships (map)
    - Count Descendants (top 5)
    - Isolate the full family tree of each of the top 5 roots (subset)
    - Built a directed graph (nx.DiGraph) for each lineage
    - Plot all 5 trees
3. Calculated statistics: lifespan, division frequency, morphology distribution
    - Lifespan: Analyzed how long cells lived before dividing or dying
    - Division frequency: Measured how often cells divides
    - Morphology Distribution: Examined how many cells are divided vs. elongated

# Results
Lineage Tree for Root Cells
![Lineage Tree per root](results.png)

# Animation
Lineage Tree Animations

![lineage_anim](https://github.com/user-attachments/assets/2bd8b1b5-37f2-4219-870d-2910485e7724))
![lineage_638](https://github.com/user-attachments/assets/5ad16ca0-9bd4-4753-93e3-0b0532b9ef0a)
![lineage_526](https://github.com/user-attachments/assets/71ef291e-0886-4944-acac-a2b55b8a6aaf)
![lineage_317](https://github.com/user-attachments/assets/eb1a061b-9841-4c9a-a41a-b752154835d8)
![lineage_287](https://github.com/user-attachments/assets/2e034d7f-0534-4cdb-af8a-6a298e25f65f)

## Statistics
#### <i> LIFESPAN </i>
- Total no. of cells (for which lifespan was calculated:  8
- Avg lifespan of all cells: 				294.95
- Standard Deviation: 					802.97
- Shortest lived cell: 					0.0
- Longest lived cell: 					2282.0

Avg lifespans per lineage:
- Root id 478: 8.45 frames
- Root id 638: 8.18 frames
- Root id 287: 10.71 frames
- Root id 317: 9.14 frames
- Root id 526: 11.57 frames

#### <i> DIVISION FREQUENCY </i>
- Total Divisions: 882
- Total cells: 2282
- Division Frequency: 0.39

#### <i> MORPHOLOGY DISTRIBUTION </i>
- Morphology counts:
- Divided:   882
- Elongated: 162

Morphology percentages:
- Divided:   84.48
- Elongated: 15.52
