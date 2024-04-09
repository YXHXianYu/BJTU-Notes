# API designing and implementation

* Linglong Jin
* silentkim@126.com

## 1. Prologue

* Score
  * 50 + 50
  * like Frontend Lesson

## 2. Introduction

* What is API

## 3. API设计规范

### 3.1 四大好API原则

* Operational
  * 可用
* Expressive
  * 一看就懂
* Simple
  * 简单、基本
* Predictable
  * 易于学习、可预测

### 3.2 通用设计原则

* 简单原则
  * 单一职责
  * 声明清晰直观
* 统一原则
  * 统一命名风格、入/出参规范、错误码、版本
* 抽象原则
* 正交原则
* 兼容扩展原则
* 安全原则

### 3.3 API设计原则

* 命名规则
  * Expressive, Simple, Predictable
* 类型数据和默认值
  * 注：如何确保多个系统同时读取和修改同个数据？
    * 双缓冲：最优解
    * 事件队列：需要加锁

## 4. API Design Pattern

* Standard Interface
  * Get, List, Create, Replace, Update, Delete

