# 2_1_1_01_Junit_测试概述

**测试分类：**

1. 黑盒测试：不需要写代码，给输入值，看程序是否能够输出期望的值
2. 白盒测试：需要写代码，关注程序的执行流程



**Junit 使用：白盒测试**

- 步骤：
  1. 定义一个测试类（测试用例）
     - 建议：
       - 测试类名：被测试的类名 Test      例如 CalculatorTest
       - 报名：xxx.xxx.test
  2. 定义测试方法：可以独立运行
     - 建议：
       - 方法名：test 测试的方法名			testAdd()
       - 返回值：void
       - 参数列表：空参
  3. 给方法加 @Test
  4. 导入 junit 依赖
  5. @Before：修饰的方法会在测试方法之前被自动执行
  6. @After：修饰的方法会在测试方法之后被自动执行
- 判定结果：
  - 绿色代表成功 
  - 红色代表失败
  - 一般我们会使用断言操作来处理结果
    - `Assert.assertEquals(期望的结果， 运算的结果);`



























