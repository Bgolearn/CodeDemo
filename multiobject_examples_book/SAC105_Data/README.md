
The folder contains the SAC-105 dataset used in this study. [Ref/Cite the Paper](https://www.sciencedirect.com/science/article/pii/S0264127524002946)

A total of 27 data points are stored in `data.csv`, including experimental test values for tensile strength and elongation.

A synthetic dataset, referred to as `Visual_samples`, is generated using an orthogonal design approach, resulting in a total of 11,767 data points. 

**Code:**  

```python
import numpy as np
import pandas as pd

# Define ranges for Bi, In, and Ti
Bi = np.arange(1.5, 5.6, 0.1)
In = np.arange(1.5, 5.6, 0.1)
Ti = np.arange(0.1, 0.8, 0.1)

# Generate a grid of Bi, In, and Ti combinations
X1, X2, X3 = np.meshgrid(Bi, In, Ti)
Visual_samples = np.vstack([X1.ravel(), X2.ravel(), X3.ravel()]).T

# Create a DataFrame
Visual_samples = pd.DataFrame(Visual_samples, columns=['Bi', 'In', 'Ti'])

# Calculate Sn and insert it as the first column
Sn = 100 - 1.5 - Visual_samples['Bi'] - Visual_samples['In'] - Visual_samples['Ti']
Visual_samples.insert(0, 'Sn', Sn)

# Print the generated DataFrame
print(Visual_samples)
```

---

For more details, refer to the resource: [video](https://www.bilibili.com/video/BV1LTtLeaEZp/?buvid=Y345CE3557236F9745C19B291052E1114B47&is_story_h5=false&mid=cKE7LXHZdUdBetZbd%2FNVln8FTQ%2FSZMtL1rElX6M3iMo%3D&plat_id=240&share_from=ugc&share_medium=iphone&share_plat=ios&share_source=WEIXIN&share_tag=s_i&timestamp=1726650391&unique_k=fyJEJqG&up_id=3546615870654962).

