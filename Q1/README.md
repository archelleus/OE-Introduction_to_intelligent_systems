# Q1: Washing Machine Cycle Time using Fuzzy Logic

## Objective
Design a fuzzy logic system to determine washing machine cycle time based on dirt level and load size.

## Inputs
1. Dirt Level (0–10)
   - Low
   - Medium
   - High

2. Load Size (0–10)
   - Small
   - Medium
   - Large

## Output
- Cycle Time (0–60 minutes)
  - Short
  - Normal
  - Long

## Methodology
- Type: Mamdani Fuzzy Inference System
- Membership Functions: Triangular (trimf)
- Defuzzification: Centroid method

## Membership Functions
- Dirt Level: Low [0 0 3], Medium [2 5 8], High [6 10 10]
- Load Size: Small [0 0 4], Medium [3 5 7], Large [6 10 10]
- Cycle Time: Short [0 0 20], Normal [15 30 45], Long [40 60 60]

## Rule Base
1. IF Dirt is Low AND Load is Small → Short
2. IF Dirt is Low AND Load is Medium → Normal
3. IF Dirt is Medium AND Load is Small → Normal
4. IF Dirt is Medium AND Load is Large → Long
5. IF Dirt is High AND Load is Medium → Long
6. IF Dirt is High AND Load is Large → Long
7. IF Dirt is Low AND Load is Large → Normal

## Tools Used
- MATLAB Fuzzy Logic Toolbox

## Output
- Rule Viewer used to analyze system behavior
- Example:
  - Input: Dirt = 7, Load = 8
  - Output: Long cycle time (~55 min)

## Conclusion
The fuzzy system successfully models washing conditions and provides an appropriate cycle time using linguistic rules.
