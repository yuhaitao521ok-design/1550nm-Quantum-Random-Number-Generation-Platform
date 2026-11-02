# 1550nm 量子随机数生成平台

> 1550 nm Quantum Random Number Generation Platform

基于 1550 nm 波段光量子噪声的量子随机数生成（QRNG）平台，用于产生具备物理不可预测性的真随机数，
并对外提供随机数服务接口。

## 项目状态

仓库初始化阶段，仅包含本说明文档。后续模块将按下面的规划逐步加入。

## 目标

- 采集 1550 nm 光源（如 DFB 激光器 / ASE 光源）经探测后的量子噪声信号
- 对原始采样数据进行熵源评估、后处理（提取器 / 随机性萃取）与统计检验
- 输出满足 NIST SP 800-90B / AIS-31 等标准要求的随机数
- 提供可调用的随机数服务（本地 SDK 与网络接口）

## 规划中的目录结构

```text
.
├── README.md
├── docs/              # 设计文档、原理说明、测试报告
├── hardware/          # 1550 nm 光路与采集硬件配置、驱动
├── acquisition/       # 信号采集与原始数据落盘
├── entropy/           # 熵源建模与熵估计
├── postprocess/       # 后处理 / 随机性提取算法
├── tests/             # 统计检验（NIST STS、Dieharder 等）与单元测试
└── service/           # 随机数服务接口（API / SDK）
```

## 快速开始

当前仓库尚无可执行代码。克隆后即可开始开发：

```bash
git clone https://github.com/yuhaitao521ok-design/1550nm-Quantum-Random-Number-Generation-Platform.git
cd 1550nm-Quantum-Random-Number-Generation-Platform
```

## 文档

- 原理与系统设计：`docs/`（待补充）
- 测试与检验报告：`docs/`（待补充）

## 许可证

待定（TBD）。
