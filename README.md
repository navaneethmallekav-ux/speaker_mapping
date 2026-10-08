# Optimized Speaker Placement System

A mathematical optimization project that determines the optimal placement of speakers in a rectangular room to achieve desired audio coverage using greedy set-cover algorithms.

## Project Overview

Given:
- room dimensions (length × width)
- speaker effective audio reach (radius)
- target coverage percentage

The system computes:
- discretized room grid
- Euclidean distance matrices
- binary coverage matrices
- optimized speaker positions using greedy selection
- final visualization of room coverage

## Files

- `Optimized Speaker Placement.ipynb` — main notebook containing the implementation, explanation, and visualizations.

## How to Run

### In Google Colab
Upload the notebook to Colab and run the cells block by block.

### In Jupyter Notebook
```bash
pip install numpy matplotlib
jupyter notebook Optimized_Speaker_Placement_MFAD_Orange_Project.ipynb
```

## Parameter Setup

Update the values in the `USER INPUTS` section:

```python
ROOM_LENGTH = 12.0
ROOM_WIDTH = 8.0
SPEAKER_RADIUS = 3.0
GRID_SPACING = 0.5
MIN_COVERAGE = 95.0
```

## Core Idea

The project uses:
- Euclidean distance between speakers and room points
- binary coverage conditions using the effective radius
- greedy optimization to choose the speaker covering the largest number of uncovered points
- plotting to visualize the final layout and coverage improvement

## Output

The notebook produces:
- number of speakers needed
- recommended speaker coordinates
- achieved room coverage percentage
- room layout with coverage circles
- coverage improvement graph across speaker additions

## Possible Extensions

- obstacles and walls
- directional speaker coverage
- 3D placement
- variable speaker strength
- weighted priority regions
- more advanced optimization algorithms

## License

For educational and mini-project use.
