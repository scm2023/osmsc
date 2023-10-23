OSMsc 
====
![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue?style=plastic)
![PyPI](https://img.shields.io/pypi/v/osmsc?style=plastic)
![PyPI - Wheel](https://img.shields.io/pypi/wheel/osmsc?style=plastic)
![PyPI - Implementation](https://img.shields.io/pypi/implementation/osmsc?style=plastic)
![GitHub repo size](https://img.shields.io/github/repo-size/ruirzma/osmsc?style=plastic)
![GitHub repo file count](https://img.shields.io/github/directory-file-count/ruirzma/osmsc?style=plastic)
![PyPI - License](https://img.shields.io/pypi/l/osmsc?style=plastic)



*Updated September 23, 2023*

<font color=green size=4> This repo develops an easy-to-use Python package, named OSMsc, to improve the availability, consistency and generalizability of urban semantic data.(一款可以快速生成全球任意城市3D模型的应用，更多使用案例可在https://github.com/ruirzma/osmsc-examples 获取)</font>

<font size=10> **OSMsc v0.2.0 is coming!** </font>



![](abigail-keenan-RaVcslj475Y-unsplash.jpg)

<p align = "center"> 
Photo by <a href="https://unsplash.com/@akeenster?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Abigail  Keenan</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
</p>


The main contributions of OSMsc:
* Construct semantic city objects based on the public dataset (OpenStreetMap), and apply geometric operations to build more complete city objects;
  内部集成了OSM数据的自动化下载，仅需几行简单的代码，即可完成城市对象的构建;
* Fuse 3D and tag information from multiple data sources through the spatial analysis between OSMsc layers and other non-OSM data layers （轻松融合外部3D或者文本数据，丰富OSM城市对象的信息）;
* Propose the semantic connector(UrbanTile), and supplement the spatial semantics （城市模型内部的对象可以添加空间语义，彼此的空间关系可以查询或者推测出来）;
* Output the CityJSON-formatted semantic city models （可以输出CityJSON或者html的可视化文件，CityJSON格式文件可以由https://ninja.cityjson.org 查看）.



![workflow](osmsc_workflow_updated.png "workflow")
<p align = "center"> OSMsc workflow</p>

<div align=center>
<img src="https://github.com/ruirzma/osmsc/blob/main/examples/Paris_cityjson.png" width="800" height="480"> 
</div>
<p align = "center"> Semantic city model generated by OSMsc</p>

### Installation


Install from [Github](https://github.com/ruirzma/osmsc)

`git clone https://github.com/ruirzma/osmsc.git`

`cd osmsc/`

`pip install .` or `python setup.py install`


Install from [PyPi](https://pypi.org/project/osmsc/)

`pip install osmsc`


Note: 

* OSMnx should be installed before OSMsc, installation errors of OSMnx could be resolved in the latest OSMnx [documentation](https://osmnx.readthedocs.io/en/stable/index.html).

* If installing OSMnx manually, pls download the Python extension packages (Rtree, GDAL, Fiona, rasterio, etc.) from [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/) for Windows and [Homebrew🍺](https://brew.sh/) for MacOS.


### Examples


[OSMsc demonstration notebooks](https://github.com/ruirzma/osmsc/tree/main/examples)


## Citation
If you use OSMsc in scientific work, I kindly ask you to cite it:

```bibtex
@article{doi:10.1080/13658816.2023.2266824,
author = {Rui Ma, Jiayu Chen, Chendi Yang and Xin Li},
title = {OSMsc: a framework for semantic 3D city modeling using OpenStreetMap},
journal = {International Journal of Geographical Information Science},
volume = {0},
number = {0},
pages = {1-26},
year = {2023},
publisher = {Taylor & Francis},
doi = {10.1080/13658816.2023.2266824},
URL = {https://doi.org/10.1080/13658816.2023.2266824},
eprint = {https://doi.org/10.1080/13658816.2023.2266824}}
```


### Reference
    1. Geoff Boeing, OSMnx, https://github.com/gboeing/osmnx
    2. Nick Bristow, OSMuf, https://github.com/AtelierLibre/osmuf
    3. Joris Van den Bossche, GeoPandas, https://github.com/geopandas/geopandas

