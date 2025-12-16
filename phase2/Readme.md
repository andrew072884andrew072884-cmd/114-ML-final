## Data Preprocessing
Run `preprocess_data.py` to prepare the data.
This script transforms the raw prediction file from `model_output/val/predictions.csv` into the input format required for Stage 2 at `phase2/stage2_input.csv`.

## Execution
Run the training script with command `python stage2_train_v6.py train` .
Run the evaluation script with command `python stage2_train_v6.py eval` .

### Configuration
Parameters can be modified directly within the `stage2_train_v6.py` file.

### Outputs
Upon execution, the script will generate:
1.  **Visualizations:** Two `.png` files (`loss_breakdown_v6.png` and `figure_threshold.png`).
2.  **Metrics:** A performance table displayed in the terminal.

### Others
combined_theta_trend_v6.png represents the output of the Stage 2 model trained on input from a Stage 1 model without class re-weighting or gradient clipping.
