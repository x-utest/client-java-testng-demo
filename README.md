# client-java-testng-demo

testng 的客户端，负责测试数据采。


# 成为代码贡献者

请联系 QQ：1295351490 Harmo哈莫


# 一、client-java-testng-demo项目介绍：

这是一个基于java testng的测试工具，利用这个工具，可以将自动化测试的结果数据整合起来，并在web端进行展示，包括测试报告饼图，用例增长图，bug曲线图，用例总数，运行失败的用例数，跳过用例数，失败测试方法名称，失败原因等等数据都一目了然。可以很好的帮助测试人员追踪测试数据，让领导和同事，都能看到测试同学的努力，推荐使用。


# 二、主要的依赖包:

- 1、testng：用于运行测试用例；

- 2、fastjson：用于处理json串；

- 3、zson：用于从response中获取属性的值；

- 4、HttpRequests：用于发送请求和接收响应体；

- 5、其他…… 


# 三、使用方法：

0. 注意：很重要的一点，使用之前，需要先安装xtest系统，项目官网：http://xtest.readthedocs.io/zh/latest/src/local_install.html

1. 第一步：如果你已经可以登录xtest系统，并看到系统界面的话，请先新建一个项目，并获取到配置信息（获取方法请参考xtest官网），就可以clone工程 `client-java-testng-demo` 到你的电脑本地，导入到idea中；

3. 第二步：修改配置文件中xtest_cfg.java,将project_id，app_id，app_key按照上一步获取到的配置信息进行更新，对于base_url，如果只是在本机访问xtest web端，则不用修改，否则请修改为：http：//固定IP：8009;

4. 第三步：运行工程中的`testng.xml`文件,如果可以看到控制打印日志：“测试套件执行已经开始：2018:04:13 16:17:13……”，即为正常；

5. 第四步：运行`start.java`文件，此时会把测试数据发送到服务端，如果看到控制打印日志：“恭喜，本次测试数据，提交成功了”，即为正常；

6. 第五步：执行完了`start.java`之后，你就可以到xtest的web端看看测试数据的前端展示了，cool。


# 四、其他说明：

在工程中每一个java文件中，都做了详细注释，有java基础的人，应该可以很快看懂整个流程了。由于本人java水平有限，故而可能存在缺陷，如有发现，可以帮忙参与改进，非常感谢！


# 五、相关链接：

https://github.com/x-utest/xtest-testng-sdk

感谢作者ityoung大神提供的testng测试数据获取方法。


## Author

xxk-studnet@qq.com

