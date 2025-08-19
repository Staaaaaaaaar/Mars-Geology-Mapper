# Mars Geology Mapper 火星地质地图数据处理程序

## 📖 项目简介

本项目是一个基于Python的火星地质制图分析程序集，用于处理和可视化USGS发布的火星全球地质图数据（SIM3292）。项目通过Jupyter Notebook提供交互式的地质数据分析和可视化功能，帮助研究人员和爱好者探索火星表面的地质结构特征。

## 🔧 环境要求

### 🐍 Python版本
- Python 3.7 及以上版本

### 📦 依赖包
```bash
# 地理空间数据处理
geopandas >= 0.10.0
rioxarray >= 0.12.0

# 数据分析和科学计算
pandas >= 1.3.0
numpy >= 1.21.0

# 可视化
matplotlib >= 3.5.0

# 其他工具包
pathlib (Python标准库)
collections (Python标准库)
```

## 🚀 如何开始

### 📥 第一步：克隆项目
```bash
git clone [项目仓库URL]
cd Mars-Geology-Mapper
```

### 🔨 第二步：安装依赖
```bash
# 使用pip安装依赖包
pip install geopandas rioxarray pandas numpy matplotlib

# 或使用conda安装（推荐）
conda install -c conda-forge geopandas rioxarray pandas numpy matplotlib
```

### 💾 第三步：下载数据
下载火星地质数据：

1. 点击[下载链接](http://pubs.usgs.gov/sim/3292/downloads/sim3292_database.zip)下载 `SIM3292_database.zip` 文件
2. 将压缩包解压到项目的 `resources` 文件夹下
3. 解压后的目录结构如下：
   ```
   resources/
   └── SIM3292_MarsGlobalGeologicGIS_20M/
       ├── SIM3292_Shapefiles/
       ├── Basemaps/
       ├── SIM3292_geodatabase.gdb/
       └── 其他文件...
   ```

### ▶️ 第四步：运行程序

- `scripts/geology_overview.ipynb` - 地质单元概览
- `scripts/structure_overview.ipynb` - 构造特征概览
- `scripts/basemap_overview.ipynb` - 基础底图概览
- `scripts/intersection_analysis.ipynb` - 空间交汇分析
- `scripts/geology_overlay_display.ipynb` - geology图层叠加显示
- `scripts/structure_overlay_display.ipynb` - structure图层叠加显示



## 📁 项目结构

```
Mars-Geology-Mapper/
├── README.md                    # 项目说明文档
├── scripts/                     # Jupyter Notebook分析脚本
├── resources/                   # 原始数据目录
└── output/                      # 输出结果目录
    ├── images/                  # 生成的地图图像
    └── shapefiles/              # 处理后的shp数据
```

## 📊 数据来源

本项目使用的数据来自美国地质调查局（USGS）发布的火星全球地质图：

- **数据集名称**: Geologic Map of Mars, Scale 1:20,000,000
- **发布编号**: USGS Scientific Investigations Map SIM 3292  
- **参考文献**: K.L. Tanaka, J.A. Skinner, Jr., J.M. Dohm, R.P. Irwin, III, E.J. Kolb, C.M. Fortezzo, Thomas Platz, G.G. Michael, and T.M. Hare, 2014
- **官方链接**: http://pubs.usgs.gov/sim/3292
