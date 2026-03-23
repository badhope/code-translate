# Wealth - 智能量化分析平台

![Version](https://img.shields.io/badge/version-0.3.0-blue)
![Python](https://img.shields.io/badge/python-3.10+-green)
![Vue](https://img.shields.io/badge/vue-3.4-brightgreen)

Wealth 是一个专业的智能量化分析平台，支持股票、基金等金融产品的实时数据分析、策略回测、机器学习预测和可视化展示。

## 核心功能

### 数据采集
- **AKShare 数据源**: 实时获取 A 股市场数据
- **Yahoo Finance**: 港股、美股数据支持
- **东方财富爬虫**: 基金、债券数据
- **爬虫框架**: 灵活可扩展的数据采集

### 量化分析引擎
- **技术指标**: MACD、KDJ、RSI、布林带、威廉指标
- **策略回测**: 多策略对比分析
- **组合管理**: 仓位管理、风险控制

### 机器学习预测
- **LSTM 模型**: 时间序列预测
- **Prophet 模型**: 趋势预测
- **XGBoost 模型**: 分类与回归

### 安全防护
- **反爬虫机制**: 请求频率限制、行为分析
- **数据加密**: AES-256 加密算法
- **RBAC 权限控制**: 角色权限管理

## 快速开始

### 环境要求
- Python 3.10+
- Node.js 18+
- npm 或 yarn

### 后端安装

```bash
cd wealth
pip install -r requirements.txt
```

或使用 pyproject.toml:

```bash
pip install loguru fastapi uvicorn pandas numpy akshare httpx pydantic pyecharts yfinance
```

### 前端安装

```bash
cd wealth/frontend
npm install
```

### 启动服务

```bash
# 启动后端 (端口 8000，自动检测可用端口)
cd wealth/src
python -m wealth.main

# 启动前端 (新终端)
cd wealth/frontend
npm run dev
```

### 运行测试

```bash
cd wealth/scripts
python simulation_test.py
```

## 项目结构

```
wealth/
├── src/                    # 后端源代码
│   └── wealth/
│       ├── api/           # API 路由
│       ├── data/          # 数据源
│       ├── engine/        # 量化引擎
│       ├── ml/           # 机器学习
│       ├── security/      # 安全模块
│       ├── utils/        # 工具函数
│       ├── vis/          # 可视化
│       └── main.py       # 应用入口
├── frontend/              # 前端源代码
│   └── src/
│       ├── api/          # API 调用
│       ├── assets/       # 静态资源
│       ├── components/   # 公共组件
│       ├── router/       # 路由配置
│       └── views/        # 页面视图
├── scripts/              # 脚本工具
│   ├── port_utils.py     # 端口工具
│   ├── test_data_generator.py  # 测试数据生成
│   └── simulation_test.py     # 模拟测试
└── data/                 # 数据目录
    └── test/             # 测试数据
```

## API 接口

| 方法 | 路径 | 描述 |
|------|------|------|
| GET | `/api/v1/health` | 健康检查 |
| POST | `/api/v1/stocks/quote/realtime` | 实时行情 |
| POST | `/api/v1/stocks/kline` | K 线数据 |
| POST | `/api/v1/indicators/calculate` | 计算指标 |
| POST | `/api/v1/backtest/run` | 运行回测 |
| POST | `/api/v1/strategy/list` | 策略列表 |
| GET | `/api/v1/funds/list` | 基金列表 |

完整 API 文档: http://localhost:8000/docs

## 策略说明

### MACD 策略
- 金叉买入，死叉卖出
- 参数: 快线周期、慢线周期、信号线周期

### KDJ 策略
- 超卖买入，超买卖出
- 参数: K 周期、D 周期、J 周期

### 布林带策略
- 价格触及下轨买入，上轨卖出
- 参数: 周期、标准差倍数

### 均值回归策略
- 价格偏离均值过大时反向操作
- 参数: 回归周期、偏离阈值

## 技术栈

### 后端
- **FastAPI**: 高性能 Web 框架
- **Pandas**: 数据处理
- **NumPy**: 数值计算
- **AKShare**: 金融数据
- **PyEcharts**: 图表生成

### 前端
- **Vue 3**: 渐进式框架
- **Vite**: 构建工具
- **ECharts**: 图表库
- **Vue-Echarts**: Vue 封装
- **Pinia**: 状态管理
- **Vue Router**: 路由管理

### 机器学习
- **TensorFlow/Keras**: 深度学习
- **XGBoost**: 梯度提升
- **Prophet**: 时间序列

## 页面预览

- **首页**: 市场概览、快捷入口
- **股票**: 搜索、详情、图表
- **基金**: 列表、净值、筛选
- **回测**: 策略配置、绩效分析
- **预测**: ML 模型、趋势预测
- **监控**: 系统状态、安全告警
- **预警**: 自定义规则、通知管理

## 配置说明

### 环境变量

| 变量 | 默认值 | 描述 |
|------|--------|------|
| PORT | 8000 | API 服务端口 |
| HOST | 0.0.0.0 | 服务地址 |

### 端口检测

服务启动时自动检测端口可用性，如端口被占用会自动切换到下一个可用端口。

## 开发指南

### 添加新的数据源

```python
from wealth.data.base import BaseDataSource

class MyDataSource(BaseDataSource):
    async def get_realtime(self, symbol: str):
        # 实现数据获取逻辑
        pass
```

### 添加新策略

```python
from wealth.engine.strategies import Strategy

class MyStrategy(Strategy):
    def __init__(self):
        super().__init__("my_strategy")

    def generate_signals(self, data):
        # 实现信号生成逻辑
        pass
```

### 添加新的 ML 模型

```python
from wealth.ml.predictor import BasePredictor

class MyPredictor(BasePredictor):
    def predict(self, data):
        # 实现预测逻辑
        pass
```

## 贡献指南

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

## License

本项目采用 MIT 许可证 - 参见 [LICENSE](LICENSE) 文件

## 致谢

- [AKShare](https://github.com/akfamily/akshare) - 金融数据源
- [PyEcharts](https://github.com/pyecharts/pyecharts) - Python 图表库
- [ECharts](https://github.com/apache/echarts) - 数据可视化库
- [Vue-Echarts](https://github.com/ecomfe/vue-echarts) - Vue 图表组件
