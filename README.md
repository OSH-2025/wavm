# FerriteOS

## 组名

FerriteOS

## 组徽

<img src="./assets/logo.jpg" width="400" />

## 组员

- [朱东胜 PB23111587](https://github.com/ustc1587)
- [杨博文 PB23111611](https://github.com/OwenYang1102)
- [徐家慧 PB23050897](https://github.com/Clara-X)
- [秦铭格 PB23111594](https://github.com/QinMingge)
- [袁谦朗 PB23111711](https://github.com/csjike)

## 项目进展

| 项目阶段 |      日期      |                           工作内容                           |
| :------: | :------------: | :----------------------------------------------------------: |
|   选题   | 3月2日—3月8日  | 结合往届选题和老师上课提到的选题方向，每个人选择一个感兴趣的方向进行初步调研：秦铭格，徐家慧：AI for OS；杨博文，朱东胜：Rust重构；袁谦朗：使用ray进行大模型分布式部署。 |
|   选题   |     3月8日     | 第一次线下讨论。确定了Rust重构选题，具体包括IPFS，Linux模块，微型WebAssembly虚拟机等方向。 |
|   选题   | 3月9日—3月17日 | 对Rust重构的各个方向进入深入调研，分析其价值，可行性和任务量等。 |
|   选题   |    3月17日     | 第二次线下讨论。IPFS的庞大代码库涉及DHT、Bitswap等复杂协议，异步编程复杂，基于Go的实现比较完善，重写任务量大且价值不高；Rust重构Linux目前生态不完善，参考教程少，面对C与Rust的兼容性、内核高度耦合替换难度大、调试困难等问题，风险大；WebAssembly作为一种可移植、高性能的二进制指令格式，已成为边缘计算、区块链、插件系统等领域的核心技术，用Rust实现微型WebAssembly虚拟机高度可行且价值显著，尤其在安全敏感和资源受限的场景中。因此，确立选题为微型WebAssembly虚拟机wavm。 |
|   选题   |    3月23日     | 第三次线下讨论。老师否认了基于Rust的WebAssembly解释器和运行时，同时我们对于嵌入式开发了解较少，放弃了关于freertos以及wasm虚拟机在嵌入式系统的应用等选题。经过和老师的进一步讨论，我们重新确立选题为使用Rust重构LiteOS部分模块。 |
|    调研    |    3月29日     | 第四次线下讨论。讨论了调研报告内容框架，确定了分工：朱东胜负责文档总体汇总；徐家慧写项目背景/概述；袁谦朗写立项依据；秦铭格写前瞻性、重要性分析；杨博文写相关工作。 |
| 可行性分析 |     4月4日     | 第五次线下讨论。讨论了可行性报告内容框架，确定了分工：朱东胜负责理论依据/LiteOS编译、qemu运行LiteOS模块以及文档总体汇总；秦铭格写理论依据/rust部分；徐家慧写理论依据/LiteOS部分；袁谦朗写技术依据/C调用Rust部分；杨博文写技术依据/Rust调用C部分。 |
| 源代码阅读 | 4月12日 | 第六次线下讨论。讨论并深入了解 Huawei LiteOS 源代码中 kernel 内核部分的代码结构，同时结合往届项目学习改写经验。最后对之后一周的任务做出初步规划：每人负责尝试改写 kernel/mem 目录下的一至两个文件，并对中期汇报内容进行构思。朱东胜负责 bestfit_little 中的 los_heap.c & los_memory.c；徐家慧负责 common/memstat 中的 los_memstat.c；秦铭格负责 common/multipool 中的 los_multipool.c；杨博文负责 membox 的 los_memory_dyn.c；袁谦朗负责 membox 中的 los_membox.c。 |
