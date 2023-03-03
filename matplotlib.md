## subplots layout
```python 
from matplotlib.gridspec import GridSpec
import matplotlib.pyplot as plt

fig=plt.figure()

gs=GridSpec(6,2) # 6 rows, 2 columns -> 2 on left and 3 on right

ax1=fig.add_subplot(gs[:3,0]) # First three rows, first column
ax2=fig.add_subplot(gs[3:,0]) # seond three rows, first column
ax3=fig.add_subplot(gs[:2,1]) # First two rows, second column
ax4=fig.add_subplot(gs[2:4,1]) # Second two rows, second columns
ax5=fig.add_subplot(gs[4:6,1]) # third two rows, span second columns
fig.tight_layout()
```
