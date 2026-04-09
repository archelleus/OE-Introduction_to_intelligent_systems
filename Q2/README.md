# Q2: Student Performance Prediction using ANFIS

## Objective
Develop a hybrid intelligent system combining fuzzy logic and neural networks to predict student performance.

## Inputs
1. Attendance (%)
2. Assignment Marks
3. Test Marks

## Output
- Performance Level (0–100)
  - Poor
  - Average
  - Good

## Methodology
- Model: Adaptive Neuro-Fuzzy Inference System (ANFIS)
- FIS Type: Sugeno
- Initial FIS generated using grid partition
- Membership Functions: Gaussian / Bell-shaped
- Training Method: Hybrid (Least Squares + Gradient Descent)

## Dataset
- CSV file with input-output pairs:
  [Attendance, Assignment, Test, Performance]

## Working Principle
- Fuzzy logic provides rule-based structure
- Neural network adjusts membership functions and rule parameters
- System learns from training data and improves prediction accuracy

## Training
- Epochs: 50
- Error decreases over iterations (training graph shown)

## Testing
Example:
- Input: [85, 80, 78]
- Output: ~80 (Good performance)

## Tools Used
- MATLAB Fuzzy Logic Toolbox (ANFIS Editor)

## Conclusion
The hybrid ANFIS model combines interpretability of fuzzy systems with learning capability of neural networks, resulting in accurate performance prediction.
