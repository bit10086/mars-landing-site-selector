# Mars Landing Site Selector 火星着陆区优选系统

> An intelligent system for selecting optimal landing zones on Mars, based on illumination and slope constraints.  
> 一个基于光照与坡度约束条件的智能化火星着陆区优选系统。

---

## 📁 Project Structure | 项目结构
Mars/
├── core/ # Core modules | 核心模块
│ ├── auto_landing_selction_system.ipynb # Main logic for landing site selection | 着陆点选择主逻辑
│ └── illumination_zone_selector.ipynb # Illumination zone analysis module | 光照区域识别模块
├── main.ipynb # Entry point script | 主程序入口
├── new.ipynb # Development scratchpad | 测试/开发草稿
├── data_process.py # Data preprocessing script | 数据预处理脚本
├── data/ # Raw data folder | 原始数据文件夹
├── output/ # Output results folder | 输出结果目录
├── 论文/ # Papers and documentation | 项目文档与论文
├── 参考文献/ # References | 项目参考文献
└── README.md # Project introduction | 项目介绍说明

---

## ⚙️ Core Features | 核心功能

### 🌞 Illumination Analysis 光照分析
- Compute cumulative sunlight hours per grid cell.
- 计算每个网格的累计日照时长。
- Sliding window & weighted scoring strategy supported.
- 支持滑动窗口与加权评分策略。

### 🏔 Slope Evaluation 坡度评估
- Extract terrain slope from DEM data.
- 从 DEM 数据中提取坡度。
- Support Horn method & future GPU optimization.
- 支持 Horn 算法，后续考虑 GPU 优化。

### 🧠 Candidate Selection 候选区筛选
- Combine illumination and slope constraints to rank top zones.
- 结合光照与坡度限制条件，排序最优着陆区。

---

## 🚀 How to Use | 使用方法

1. Put DEM / DIM raw data into `data/` folder.  
   将原始 DEM / DIM 数据放入 `data/` 文件夹中。
2. Run `main.ipynb` step-by-step.  
   按顺序运行 `main.ipynb`。
3. Check result in `output/`.  
   输出结果保存在 `output/` 中。
4. Customize parameters (e.g., window size, weighting λ) in core modules.  
   在 `core/` 中根据需要修改参数（如窗口大小、权重 λ 等）。

---

## ✅ TODO List | 待办功能

- [x] Add core modules 添加核心模块
- [ ] Add terrain fluctuation filter 增加地形起伏筛选指标
- [ ] Integrate crater detection (YOLO) 集成陨石坑识别模块（YOLO）
- [ ] Connect LangChain + LLM to automate selection 接入大模型自动决策模块
- [ ] Package into user-friendly agent system 打包为可交互智能体系统

---

## ✍️ Author | 作者

**王宇博 Wang Yubo**  
Email: wyb040918@163.com  
Beijing Institute of Technology | 北京理工大学  
Currently at Australian National University (ANU) | 现 ANU 交换

---

## 🛰 Vision 愿景

> "Smart terrain understanding for smarter space exploration."  
> “让地形分析更智能，为深空探索添一臂之力。”

