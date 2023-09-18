# Software Testing and Quality Assurance

> 刘海明

## 1. Introduction

* **三种错误：Fault, Error, Failure**
  * Fault: 编写时，静态的错误
  * Error: 运行时，错误的状态
  * Failure：结束后，错误的结果
  * 一份代码，可能可以编写出 **4种** 情况，分别触发上面每种情况
    * 题目：设计测试用例

* PIE (Propagation-Infection-Execution) Model
  * 内容
    * Execution: 先要运行到 fault 的代码
    * Infection: fault 会触发出 error 的状态
    * Propagation: error 会导致一个错误的结果

* Sources of Problems
  * Requirements Definition
  * Design
  * Implementation
  * Support Systems
  * Communications
  * Space Applications
  * etc.

* Most bugs are not because of mistakes in the code
  * 55% SPEC: Specification 产品说明书
  * 25% Design
  * 15% Code
  * 5% Other

* Relative cost of bugs
  * "bugs found later cost more to fix"
  * Cost to fix a bug increases **exponentially**

* What are tester goals?
  * Verification: 是否满足计划 (SPEC, build the product right)
    * Process based
  * Validation: 是否满足用户的需求 (build the right product)
    * Product based

* What is Testing?
  * Testing is the process of executinga program with **the intent of finding errors**

* **Specification**
  * The features of the software
  * The constraints on these features

* SDLC
  * Software Development Life Cycle 软件开发生命周期

* Software testing **axioms**
