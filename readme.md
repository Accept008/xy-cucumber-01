##### 使用的maven pom jar 依赖信息
    <!--自动化验收测试-->
    <dependency>
        <groupId>io.cucumber</groupId>
        <artifactId>cucumber-java</artifactId>
        <version>4.7.4</version>
        <scope>test</scope>
    </dependency>

    <dependency>
        <groupId>io.cucumber</groupId>
        <artifactId>cucumber-junit</artifactId>
        <version>4.7.4</version>
        <scope>test</scope>
    </dependency>
    
##### 操作步骤（对应 tag 1.0.1）

    1.写feature文件（calculator.feature）
---
    2.运行RunTest类,编写Step业务（CalculatorRunTest.java）
        2.1 创建Steps类（CalculatorSteps.java）
        2.2 复制在日志控制台输出的方法到Steps类(CalculatorSteps.java)
        2.3 进行Given、Then、When方法实现
---        
    3.校验业务
        运行RunTest类,日志控制台查看结果
---
    4.img
        readme-img/1.1.xx.png、readme-img/1.2.xx.png        
        

##### 添加Cucumber场景大纲（对应 tag 1.0.2）        
     复制原有测试用例，将场景(Scenario)改为场景大纲(Scenario Outline)
     
        
##### 笔记
    feature文件只是将场景(Scenario)改为场景大纲(Scenario Outline)，即值改为参数；那么step定义的Java方法是一样的
