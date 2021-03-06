## ltf library
This library is supposed to be a public library of all Token Engineering tools

## Installation
```python
pip install ltf
```

## List of all packages
```python
import ltf
help(ltf)
```

## A few examples
```python
from ltf.bondingcurves import Sigmoid
# you can run basic version with default data
sbc = Sigmoid()
sbc.fig_builder().show()
```

> `output:`
![](src/ltf/data/sbc.png)

***

> Note: You may need to use your own data

```
sbc = Sigmoid(
    csv_path='INITIAL_VALUES.csv',
    current_supply=16000000,
    zoom=1
    )
```


> Note2: The format of the csv file should be as follows

-|l|s|m|k|steps
-|-|-|-|-|-
0|l1|s1|m1|k1|steps
1|l2|s2|m2|k2|steps
2|l3|s3|m3|k3|steps
3|l4|s4|m4|k4|steps

> Example:

-|l|s|m|k|steps
-|-|-|-|-|-
0|20.8| 17	|2.10E+07	|57300	|1000
1|2	|5	|5.00E+04	|5	|1000
2|2	|5	|5.00E+05	|50	|1000
3|6	|9	|5.00E+06	|2.00E+03	|1000
