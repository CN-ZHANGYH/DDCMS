# DDCMS(Distributed Data Collaboration  Management Solution)

数据要素已成为数字经济时代最核心的生产要素，各种数据共享和交易解决方案不断出现，极大的推动了产业数字化的落地和发展。但由于缺乏统一可信的数据发布管理能力、数据传输的不透明不安全等已经无法满足日益增长的数字产业需求。

- 在多方协同合作场景下，需要一套可控、可信、可靠的面向数据管理的解决方案，降低企业管理、对接数据目录的成本。
- 在数据传输过程中，需要明确数据的提供方、使用方、使用场景、数据用量、使用时间等信息，确保个人数据可携带权的同时，实现数据传输全流程的可追溯可审计；
- 在数据传输和使用过程中，需要确保数据安全，防止数据被盗或过度暴露的同时，实现数据的可用而不可见，达到使用和挖掘数据价值的目的；

为解决以上问题，我们希望通过DDCMS(Distributed Data Collaboration  Management Solution)项目的建设，在多方协同合作场景中，面向数据管理需求，提供一套基于区块链的、安全可信、友好易用的分布式数据管理开源方案，服务于个人数据携带、企业间数据共享。在数据共享过程中，各参与方围绕数据目录展开各种业务协作，使得各参与方能够快速、高效的进行数据管理、数据需求对接、传输和使用数据的同时，确保数据的安全、可信、可靠、可追溯、可监管、可审计。

DDCMS是对DDTP实现数据要素“可信传输”、“协同生产”的落地探索和补充，在降低数据业务对接成本、提升对接效率的同时，确保数据流通过程的安全、可信、可靠。


# DDCMS角色介绍

在DDCMS中包括5中角色：数据归属方、数据提供方、数据使用方、数据见证方、系统运营方。

![DDCMS 角色](/images/roles.png)

- 数据归属方：在数据传输共享过程中，对数据使用方的数据请求进行数据授权，在数据提供方进行授权管理。
- 数据提供方：对外提供数据目录服务，负责审核数据目录使用申请及核验用户授权。
- 数据使用方：对数据归属者提供服务，并经过授权通过数据目录获取数据。
- 数据见证方：负责对数据目录的全流程进行进行审核监管，不参与具体业务。
- 系统运营方：负责对各参与方进行KYC，确保参与方可信可靠。


# DDCMS核心概念

在DDCMS中，从数据的角度而言，包括三个概念：数据提供方、数据归属业务、数据目录、
- 数据提供方：如前文所述，数据提供方对外提供数据目录，负责审核数据目录使用申请及核验用户授权。
- 数据目录：数据目录简单来说是数据提供方对其提供的数据的描述，包括数据类型、归属业务、归属机构、服务类型、数据定价、数据服务地址、数据传输协议、数据请求格式、数据响应格式等内容。
- 数据业务：数据业务是数据目录所属的系列，每个数据目录均需要挂靠在某个业务上。

它们之间的关系，可以用下图描述：

![](/images/org.png)

# DDCMS核心功能

DDCMS由三个核心功能模块构成： 统一可信的数据目录管理、可追溯审计的数据传输过程、丰富安全的数据处理组件管理。

## 数据目录管理
提供统一的数据目录管理功能，所有操作均上链存证、确保数据目录可信，提升管理和运营效率，降低接入成本。数据目录管理具体又包含用户管理、业务管理、数据目录管理、审核管理等功能。

## 数据传输过程管理
每次数据的传输过程均会上链，确保数据流通的定量、定时、定场景，实现全流程可管理可追溯可监管审计。传输过程管理具体而言，又包括授权认证、过程存证、用量统计、定价及清算等功能。

## 数据处理组件管理
提供对各种数据处理组件的管理能力，企业可按需接入和使用、避免二次开发、降低接入和使用成本。数据处理组件又包含零知识证明、联邦学习、选择性披露、隐私计算等模块。

## 项目工程
DDCMS由三个子工程构成：

### DDCMS-Contract

该项目是DDCMS的合约部分，用于对每一个相关操作进行留痕、追溯。目前包含用户管理、业务管理、数据目录管理三个功能。
请参考 
- [Github地址](https://github.com/WeBankBlockchain/Data-Brain-Contract)
- [Gitee地址](https://gitee.com/WeBankBlockchain/Data-Brain-Contract)

### DDCMS-Server

该项目是DDCMS的后端API，用于支持前端请求。
- [Github地址](https://github.com/WeBankBlockchain/Data-Brain-Server)
- [Gitee地址](https://gitee.com/WeBankBlockchain/Data-Brain-Server)

### DDCMS-Front


该项目是DDCMS的前端，用于提供友好的操作界面。
- [Github地址](https://github.com/WeBankBlockchain/Data-Brain-Front)
- [Gitee地址](https://gitee.com/WeBankBlockchain/Data-Brain-Front)


## 快速开始

具体使用方式，请参考[快速开始](http://data-brain.readthedocs.io).

## 贡献代码
欢迎参与本项目的社区建设：
- 如项目对您有帮助，欢迎点亮我们的小星星(点击项目右上方Star按钮)。
- 欢迎提交代码(Pull requests)。
- [提问和提交BUG](https://github.com/WeBankBlockchain/Data-Brain/issues)。
- 如果发现代码存在安全漏洞，请在[这里](https://security.webank.com)上报。


## License
![license](http://img.shields.io/badge/license-Apache%20v2-blue.svg)

开源协议为[Apache License 2.0](http://www.apache.org/licenses/). 详情参考[LICENSE](../LICENSE)。
