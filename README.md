# Awesome-Earth-Observation-Analytics

# 顶级地球观测分析平台生态系统

**精选 SaaS 产品与开源 GitHub 项目列表**
*聚焦卫星图像分析、变化检测、植被监测与环境智能*
**最后更新：2026 年 9 月**

本仓库追踪**地球观测分析**领域的知名 **SaaS 平台**与**开源项目**。这些工具帮助分析师、研究人员和企业从卫星图像中提取可操作洞察——监测植被健康、检测环境变化、评估灾害影响，并支持数据驱动的决策。

**示例**包括 UP42、Descartes Labs、Orbital Insight、Picterra、EOS Data Analytics、Satellogic Insights、SkyWatch、Planet Insights、SpaceKnow 和 EarthDaily Analytics（该领域的领先者）。

**开源重点**：地球观测领域拥有**极其丰富的开源生态**——这得益于 ESA 哥白尼计划的免费开放数据政策。与许多企业软件类别不同，开源工具不仅存在，而且在灵活性和数据主权方面往往优于商业产品。本列表重点收录**可自托管的处理引擎**、**变化检测框架**和**数据立方体工具**——适合需要完全掌控分析流程的研究团队和开发者。

欢迎贡献！提交 PR 以添加/更新条目。保持描述事实性，并链接到官方网站。

## 目录

- [SaaS/托管平台](#saas托管平台)
- [开源 GitHub 项目](#开源github项目)
- [如何贡献](#如何贡献)
- [免责声明](#免责声明)

## SaaS/托管平台

- **[UP42](https://up42.com/)**
  地球观测数据平台和市场。提供来自多个供应商的卫星和航空影像访问，以及用于处理和分析的 API。支持快速原型设计和生产级工作流。

- **[Descartes Labs](https://descarteslabs.com/)**
  地理空间分析平台，结合卫星影像与机器学习，应用于农业、林业和环境监测。

- **[Orbital Insight](https://orbitalinsight.com/)**
  地理空间分析平台，使用 AI 大规模分析卫星和航空影像。专注于经济活动监测、供应链情报和基础设施追踪。

- **[Picterra](https://picterra.ch/)**
  地理空间 AI 平台，用于检测卫星和航空影像中的物体和变化。无需代码即可训练模型，适用于基础设施监测、农业和环境分析。

- **[EOS Data Analytics](https://eos.com/)**
  卫星数据分析平台，专注于农业、林业和环境监测。提供作物健康监测、产量预测和土地覆盖分类。

- **[Satellogic Insights](https://satellogic.com/)**
  高频卫星图像和分析服务。提供每日重访能力，用于变化检测和环境监测应用。

- **[SkyWatch](https://skywatch.com/)**
  地球观测数据平台，提供卫星影像 API 和数据分析服务。简化了从多个供应商获取影像的流程。

- **[Planet Insights](https://www.planet.com/)**
  Planet 公司的分析平台，基于其每日卫星图像星座提供变化检测、植被监测和物体检测服务。

- **[SpaceKnow](https://spaceknow.com/)**
  卫星图像分析平台，专注于经济指标、基础设施监测和异常检测。

- **[EarthDaily Analytics](https://earthdaily.com/)**
  地球观测分析平台，提供每日卫星图像处理和分析服务，覆盖农业、环境和基础设施领域。

## 开源 GitHub 项目

- **[satellite-ndvi-pipeline](https://github.com/DMN-SOLUTIONS/satellite-ndvi-pipeline)**
  自动化卫星图像处理管道，带 QGIS 插件。从 AWS 开放数据下载免费 Sentinel-2 影像，计算 NDVI（植被）、NDWI（水体）和 NBR（火烧迹地）指数，矢量化为 GeoJSON 多边形，并检测日期之间的变化。支持 QGIS 暗色主题 UI、日期选择器、变化检测标签页和可配置阈值的警报系统。可通过 AWS SAM 部署为 SaaS API（API Gateway + Lambda + S3）。**开源** 。

- **[gdalcubes](https://github.com/appelmar/gdalcubes)**
  将地球观测图像集合转换为按需数据立方体的 R 包。支持从 STAC 目录或本地文件创建图像集合，执行空间聚合（`aggregate_space`）、时间聚合（`aggregate_time`）和波段选择。支持 Sentinel-1/2、Landsat 等格式。与 Xarray 生态系统集成，适合构建可扩展的 EO 数据立方体工作流。**开源（R 包）** 。

- **[unbihexium](https://github.com/unbihexium-oss/unbihexium)**
  综合性地球观测分析框架，包含 12 个功能领域：风险与防御（危险分析、海事感知）、增值影像（DSM、DEM、正射校正）、卫星影像特征（立体、全色锐化）、分辨率与元数据 QA、雷达与 SAR（幅度、相位、InSAR）。支持 PyPI/Conda/Docker 安装，GPU 加速（10-50 倍推理速度提升）。提供模型库（检测、分割）和光谱指数模型。CLI 支持模型浏览、训练和推理。**开源** 。

- **[LIGHT Change Detection](https://github.com/Pavlo-Andrianatos/LIGHT-Latent-space-change-detectIon-via-Gradient-free-tHreshold-opTimisation)**
  半监督卫星图像变化检测框架，发表于学术论文。在 U-Net 编码器的潜在特征空间中操作，通过无梯度优化方法（CMA-ES、PSO、GA、MCMC）自动学习阈值。仅需 10-15 个标注变化图像即可获得竞争性结果。在 Vaihingen、HRSCD 和 SyntheWorld 数据集上验证。**开源（CC BY-NC-SA 4.0）** 。

- **[Gaia](https://github.com/alonsoggpablo/gaia_rs)**
  开源工具，用于管理和分析哥白尼 ESA 卫星图像。在哥白尼数据空间生态社区论坛上发布 。

- **[stac2cube](https://github.com/BaturalpArisoy/stac2cube)**
  可扩展的 Sentinel-2 数据立方体生成包，基于 Xarray 工作流。统一云掩膜（s2cloudless）、配准（AROSICS）和超分辨率（SEN2SR）到单一管道。支持 HPC 集群和本地工作站，提供增量更新能力。**开源（Python 包）** 。

- **[Brazil Data Cube](https://github.com/brazil-data-cube)**
  巴西国家空间研究院（INPE）开发的地球观测数据立方体项目。包含三个已注册软件系统：**TerraCollect**（土地覆盖样本采集与分析平台）、**WSAS**（Web 样本分析服务，集成时间序列分析方法）、**WCPMS**（Web 作物物候指标服务，计算 EO 数据立方体的物候指标）。支持 PRODES 和 TerraClass 等巴西国家环境监测项目。**开源** 。

- **[PICANTEO](https://github.com/）**
  模块化遥感变化检测框架。支持建筑检测（二值语义分割）和变化检测（Siamese 架构直接双时相输入）。提供基于 MA-Net 骨干的 UNet 基线模型，在 BDA 数据集上训练，优化跨传感器 VHR 建筑分割鲁棒性。**开源** 。

### 其他强开源选项

- **数据获取与处理**：**eoreader**（传感器无关的遥感 Python 库，支持光学和 SAR 传感器）、**raster4ml**（机器学习地理空间栅格处理库）。
- **数据立方体**：**gdalcubes**（R 包，按需数据立方体）、**stac2cube**（Python，Sentinel-2 数据立方体）。
- **变化检测**：**LIGHT**（半监督，无梯度优化）、**PICANTEO**（模块化框架）。
- **数据源**：**Copernicus Data Space Ecosystem**（免费开放 Sentinel 数据访问，34 PB+ 存档）、**NASA Earthdata**（EarthData Search、AppEEARS、LP DAAC）。

**构建自定义系统的框架**：结合 **satellite-ndvi-pipeline** 或 **gdalcubes** 进行核心图像处理，**LIGHT** 或 **PICANTEO** 进行变化检测，**stac2cube** 构建可扩展数据立方体，**QGIS** 进行可视化。添加 **Copernicus Data Space Ecosystem** 作为免费数据源，**PostgreSQL/PostGIS** 进行空间数据存储。

## 如何贡献

1. Fork 仓库。
2. 在 `README.md` 中添加/编辑条目（遵循现有格式）。
3. 包含：名称、链接、1-2 句描述，以及是 SaaS 还是开源。
4. 提交 PR 并附简短说明。

如果你觉得这个仓库有用，请点星！

## 免责声明

- 这是一个**社区精选**列表——并非详尽无遗，也不构成认可。
- 地球观测分析平台处理可能敏感的位置和环境数据；确保遵守相关数据许可和隐私法规。
- 自托管开源解决方案需要适当的计算资源（GPU 加速可选但推荐）、存储基础设施和持续维护。

---

**为遥感分析师、环境科学家、地理空间开发者和农业技术团队打造。**
让地球观测分析更开放、透明、可扩展。
