# Selective Search Implementation for Python

This is a simple Selective Search Implementation for Python

## Declaration

This project is forked from [AlpacaDB/selectivesearch](https://github.com/AlpacaDB/selectivesearch "AlpacaDB/selectivesearch") which is originally coded in python2.

I convert it to be python3 compatible. However, no guarantee it works properly. 
Use it at your own risk!

## Install

You can just paste selectivesearch folder to your project, and import it.
No need to install.

## Usage

It is super-simple.

```python
import skimage.data
import selectivesearch

img = skimage.data.astronaut()
img_lbl, regions = selectivesearch.selective_search(img, scale=500, sigma=0.9, min_size=10)
regions[:10]
=>
[{'labels': [0.0], 'rect': (0, 0, 15, 24), 'size': 260},
 {'labels': [1.0], 'rect': (13, 0, 1, 12), 'size': 23},
 {'labels': [2.0], 'rect': (0, 15, 15, 11), 'size': 30},
 {'labels': [3.0], 'rect': (15, 14, 0, 0), 'size': 1},
 {'labels': [4.0], 'rect': (0, 0, 61, 153), 'size': 4927},
 {'labels': [5.0], 'rect': (0, 12, 61, 142), 'size': 177},
 {'labels': [6.0], 'rect': (7, 54, 6, 17), 'size': 8},
 {'labels': [7.0], 'rect': (28, 50, 18, 32), 'size': 22},
 {'labels': [8.0], 'rect': (2, 99, 7, 24), 'size': 24},
 {'labels': [9.0], 'rect': (14, 118, 79, 117), 'size': 4008}]
```

See also an example/example.py which generates :
![alt tag](https://github.com/AlpacaDB/selectivesearch/raw/develop/example/result.png)

## Blog
- EN: http://blog.alpaca.ai/open-source-pure-python-selective-search-and-advanced-object-recognition-with-labellio/
- JP: http://blog-jp.alpaca.ai/entry/2015/08/05/235408
