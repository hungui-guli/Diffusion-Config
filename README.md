```markdown
# ⚙️ DDPM Model Config

| Key               | Value                    |
|-------------------|--------------------------|
| Backbone          | U-Net (128 → 1024 → 128) |
| Timesteps         | 1000                     |
| Beta Schedule     | Linear 1e-4 → 2e-2       |
| Loss              | MSE on ε-prediction      |
| Optimizer         | AdamW, 2e-4, EMA 0.9999  |
| Batch             | 128 (A100×8)             |
| Epochs            | 1.5 M steps              |
| Precision         | FP16                     |
| Sampling          | DDPM or DDIM 50          |
```
