# Baseline Model

**[Notebook](2_BaselineModel/baseline_model.ipynb)**

## Baseline Model Results

### Model Selection
- **Baseline Model Type:** [Linear Regression]
- **Rationale:** [Linear Regression was selected as the baseline model because it is a simple, interpretable, and widely used algorithm for regression tasks. Additionally, its coefficients allow direct interpretation of how each feature influences the target variable, which supports transparency and business decision-making.]

### Model Performance
- **Evaluation Metric:** [R²]
- **Performance Score:** [83.4%]
- **Cross-Validation Score:** [Mean and standard deviation of CV scores, e.g., 0.82 ± 0.03]

### Evaluation Methodology
- **Data Split:** [Train/Validation/Test split ratios, e.g., 70/15/15]
- **Evaluation Metrics:** [List all metrics used and justify why they are appropriate for this problem]

### Metric Practical Relevance
[5. Real-World Translation to Decision-Making

Because the dependent variable is log_Umsatz, coefficients can be interpreted approximately as percentage changes.

Examples:

Weekend coefficient (0.1186)
→ ~11.9% higher revenue on weekends.

New Year (0.6601)
→ ~66% revenue increase.

Easter (0.2102)
→ ~21% increase.

Lag variables
→ Revenue persistence (today’s sales depend on yesterday’s sales).

How This Supports Business Decisions!

With 83.4% explanatory power, the model enables:

- Revenue forecasting

- Staff scheduling

- Inventory planning

- Event-based demand preparation

- Product group performance comparison

- Seasonal demand optimization

It provides reliable quantitative evidence of:

- Which events drive revenue spikes

- How strong weekend effects are

How persistent daily sales patterns are]

## Next Steps
This baseline model serves as a reference point for evaluating more sophisticated models in the [Model Definition and Evaluation](2_BaselineModel/baseline_model.ipynb) phase.
