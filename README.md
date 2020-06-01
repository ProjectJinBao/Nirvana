# Nirvana  涅槃，超脱一切烦恼的境界
通过UI界面与用户友好交互，提供统一的文档入口，根据接口文档自动生成测试用例，是集测试用例管理与接口自动化为一体的可视化智能平台！

## 背景
 
  中国互联网行业发展迅猛，在这日益变革的过程中互联网技术也在不断更新，随着技术的演进，前后端分离构架变的越来越流行。前后端分离使后端专注于数据处理和定义所需要的接口，前端负责数据的展示和交互，大大细化了开发者的职责，提高了开发效率。作为测试，只依赖前端进行限制已经完全不能满足系统的安全要求，需要在后端进行同样的控制，在这种情况下就需要从接口层面进行验证。但在实际工作开展中却困难重重：
  
- 没有统一的入口：有各种文档维护方式，如 wiki、word、gitlab、swagger等，甚至没有接口文档
- 接口经常发生变化：如增加了参数、参数名改变、path变更等
- 传统的接口测试框架使用成本很高，效率很低
- 每个写接口自动化的人都有一套自己的体系，推广体系成本高，最后导致维护成本高
- 全自动化实现对测试人员代码能力有要求，门槛高、受众群体小


## 产品介绍
### 统一入口
免费的开源软件GitLab，由统一入口来管理接口文档，实现多人协作、历史可追溯、有变动即更新的文档管理模式。  
### 接口规范
OpenAPI Specification(OAS) 定义了一个标准的、语言无关的 RESTful API 描述格式，支持规范版本 OpenAPI 3.0。
### 测试框架
框架使用 HttpRunner，轻松实现 HTTP(S) 的各种测试，满足自动化测试、性能测试、线上监控、持续集成等多种测试需求。
### 测试用例
根据接口文档自动生成测试用例，保障测试用例的统一性和可维护性。支持全局变量、环境变量和函数脚本，RESPONSE支持丰富的校验机制。
### UI交互
采用UI界面来管理测试用例，让测试不会迷失在测试用例的海洋中，更多的把关注点放在测试数据的构建上。
### 测试报告
测试结果统计报告简洁清晰，附带详尽统计信息和日志记录。

## 功能介绍

<details>
  <summary><mark>变量</mark></summary>
  <p>
   
#### 全局变量（Global variables）  
全部变量的作用域是在整个工作空间,作为系统默认的变量存在。  


#### 环境变量（Environment variables）  

环境变量的作用域是用例执行时所选择的环境内，如果一个key即存在全局变量中，又存在环境变量中，优先使用环境变量的值。    


###### *环境 在实际测试中会有多套环境，包括测试环境、预生产环境、或者针对不同版本的环境，每个环境对应的一些变量如请求地址、用户信息和中间件地址等都不相同，为了避免每测试一个环境都要手动修改相关数据，引入环境概念。*

#### 引用变量
通过特殊符号$引用变量，例如$Variables</p>

</details>
