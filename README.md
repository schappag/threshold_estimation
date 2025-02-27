# Threshold Estimation

This repository contains Python code for estimating breakpoints in piecewise linear functions, which consist of either two or three linear segments plus noise. A classic application of this method is the estimation of anaerobic thresholds in physiological data.

## Overview

The code provided in this repository was used in the study:

**The relationship and agreement between systemic and local breakpoints in locomotor and non-locomotor muscles during single-leg cycling**
(https://www.frontiersin.org/journals/physiology/articles/10.3389/fphys.2025.1465344/full?utm_source=email-sig&utm_medium=email&utm_content=100_VIEWS&utm_campaign=imp_mile_2024_fall_en_aut-ww)
Authored by:
- Markus Tilp
- Nina Mosser
- Gudrun Schappacher-Tilp (repo owner)
- Annika Kruse
- Philipp Birnbaumer
- Gerhard Tschakert


## Features

- **Breakpoint Estimation**: Detects breakpoints in piecewise linear functions.
- **Application**: Particularly useful for physiological data to estimate anaerobic thresholds.
- **Noise Handling**: Efficiently handles noise in the data.

## Requirements

- Python 3.6 or later
- Required Python packages:
  - numpy
  - pandas
  - scipy
  - matplotlib

You can install the required packages using:

```bash
pip install numpy pandas scipy matplotlib
```

## Example

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from your_module import inflection_points_EMG

# Example usage
filename = 'path_to_emg_file.csv'
titlename = 'Example Title'

# Estimate breakpoints
combined_short_table = inflection_points_EMG(filename, titlename)

# Display results
print(combined_short_table)
```

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

## License

This project is licensed under the MIT License. See the [LICENSE](https://opensource.org/license/mit) file for details.

## Contact

For any inquiries or issues, please contact the authors of the study or open an issue in this repository.
