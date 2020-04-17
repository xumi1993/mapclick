# mapclick
Select points on a map via Matplotlib UI

![](https://raw.githubusercontent.com/xumi1993/blog.post/master/static/img/mappick/mappick.gif)

## Installation
```
pip install mapclick
```

or
```
git clone https://github.com/xumi1993/mapclick.git
cd mapclick
pip install .
```

## Example
```python
from mapclick import MapPoint
mp = MapPoint()
mp.generate_map(100, 106, 21.5, 24.5, elev=True, resolution=8, nation=False, xa=0.5, ya=0.5)
mp.plot_line('/path/to/province.cn', linewidth=0.5, color='k')
mp.plot_line('/path/to/faults.ftd', linewidth=1, color=(0/255, 105/255, 167/255))
mp.plot_station('/path/to/stations.lst')
plt.show()
```
