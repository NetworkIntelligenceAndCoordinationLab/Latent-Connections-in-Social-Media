# Temporal fingerprints: Identity matching across fully encrypted domain

Shahar Somin, Keeley Erhardt, Tom Cohen, Jeremy Kepner, Alex Pentland

## Overview

The demo showcases a novel approach for matching profiles across different social media platforms (Twitter, Telegram, Instagram) through individual *temporal fingerprints*. This methodology requires only temporal metadata and works without access to network structure or user-generated content, making it especially applicable to encrypted domains.

## Repository Structure

```
├── demo_identity_matching_short.ipynb          # Main demonstration notebook
├── hashed_identity_matching_demo_20240608_20240615.csv  # Dataset with posting activity metadata
└── README.md                                   # This file
```

## Dataset


- **Time period**: June 8-15, 2024 (1 week)
- **84,786 posts**:
    - Twitter: 44,627
    - Telegram: 38,838
    - Instagram: 1,321
- **232 users** (out of 266 in full dataset):
    - Instagram: 15
    - Telegram: 108
    - Twitter: 109
- **123 Identities** (out of 131 in full dataset) 
- **Schema**:
  - `creator_name`: Hashed profile identifier
  - `platform_type`: Social platform (twitter, telegram, instagram)
  - `creation_time`: Post timestamp in UTC
  - `label`: Ground truth identity group (manually verified)

## Usage

1. **Prerequisites**: 
   - Python 3.x
   - Required packages: `pandas`, `scipy`, `matplotlib`

2. **Run the demo**:
   ```bash
   jupyter notebook demo_identity_matching_short.ipynb
   ```

## Citation

If you find this work useful, please consider citing the original paper: 

@article{somin2025temporal,
  title={Temporal fingerprints for identity matching across fully encrypted domains},
  author={Somin, Shahar and Erhardt, Keeley and Cohen, Tom and Kepner, Jeremy and Pentland, Alex‘Sandy’},
  journal={Nature Communications},
  volume={16},
  number={1},
  pages={1--11},
  year={2025},
  publisher={Nature Publishing Group}
}
