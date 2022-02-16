Agent 配置
==================
参数表
+++++++++++++++++

- **dongtai.app.name**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.app.name=<application name>`` 
   * - 参数类型
     - String
   * - 来源
     - 配置文件
   * - 可选参数
     - 格式：中文、英文字母大小写、数字、@等组合，长度20以内，名称保证唯一
   * - 默认值
     - Demo Project
   * - 参数说明
     - 项目名称

- **dongtai.app.create**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%
   
   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.app.create=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 配置文件
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - false
   * - 参数说明
     - 是否在管理服务器上自动创建项目

- **dongtai.app.version**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.app.version=<v1.1.0>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - 应用版本号
   * - 默认值
     - v1.0
   * - 参数说明
     - 当配置该参数启动时，会自动创建项目及版本
     
- **dongtai.debug**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.debug=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 命令行参数
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - false
   * - 参数说明
     - 开启后检测本地临时目录中是否存在核心检测引擎存在，加载本地检测引擎并启动

- **iast.mode**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.mode=<hunter or normal>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - ``hunter`` ｜ ``normal``
   * - 默认值
     - normal
   * - 参数说明
     - 漏洞检验模式，hunter模式漏洞多、误报率高，normal模式漏洞相对少、误报率低

- **iast.server.mode**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.server.mode=<local or remote>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - ``local`` ｜ ``remote``
   * - 默认值
     - remote
   * - 参数说明
     - local模式支持单漏洞验证、项目漏洞批量验证、POST请求包展示、污点位置及污点值展示等功能

- **iast.proxy.enable**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.proxy.enable=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 配置文件
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - false
   * - 参数说明
     - HTTP代理模式是否启用

- **iast.proxy.host**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.proxy.host=<ip>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - 代理的域名 (IP)
   * - 默认值
     - null
   * - 参数说明
     - HTTP 代理的域名 (IP)

- **iast.proxy.port**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.proxy.port=<port>`` 
   * - 参数类型
     - String
   * - 来源
     - 配置文件
   * - 可选参数
     - 端口 (1 to 65535)
   * - 默认值
     - 80
   * - 参数说明
     - HTTP 代理的端口

- **iast.engine.delay.time**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.engine.delay.time=<10>`` 
   * - 参数类型
     - 整型数字
   * - 来源
     - 配置文件
   * - 可选参数
     - 任意整型数字
   * - 默认值
     - 0
   * - 参数说明
     - 延迟启动功能，单位：秒

- **iast.dump.class.enable**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.dump.class.enable=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 配置文件
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - false
   * - 参数说明
     - 是否 dump 修改后的字节码

- **iast.dump.class.path**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.dump.class.path=</tmp/iast-class-dump/>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - 任意有权限路径
   * - 默认值
     - /tmp/iast-class-dump/
   * - 参数说明
     - dump 字节码的路径

- **dongtai.server.url**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.server.url=`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - URL 格式
   * - 默认值
     - https://openapi.iast.io
   * - 参数说明
     - Server URL
     
- **dongtai.server.token**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.server.token=`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - 字符串
   * - 默认值
     - user token
   * - 参数说明
     - Server Token

- **iast.allhook.enable**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Diast.allhook.enable=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 配置文件
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - false
   * - 参数说明
     - 开启全量HOOK模式

- **response.length**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Dresponse.length=<1000>`` 
   * - 参数类型
     - 整形数字
   * - 来源
     - 配置文件
   * - 可选参数
     - 大于0的整形数字
   * - 默认值
     - 无
   * - 参数说明
     - 当配置该参数启动时，会改变 agent 获取应用的 http 请求响应体的长度
     
- **dongtai.log**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.log=<true or false>`` 
   * - 参数类型
     - Boolean
   * - 来源
     - 配置文件
   * - 可选参数
     - ``true`` ｜ ``false``
   * - 默认值
     - true
   * - 参数说明
     - 是否把日志输出到本地文件

- **dongtai.log.path**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.log.path=/tmp`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - 任意有读写权限的目录
   * - 默认值
     - agent.jar 当前目录
   * - 参数说明
     - 指定日志文件所在目录
     
- **dongtai.log.level**

.. list-table::
   :widths: 4 20
   :header-rows: 1
   :width: 100%

   * - 属性
     - 值
   * - 生效方式
     - 启动时添加 ``-Ddongtai.log.level=<1000>`` 
   * - 参数类型
     - 字符串
   * - 来源
     - 配置文件
   * - 可选参数
     - info,debug
   * - 默认值
     - info
   * - 参数说明
     - 指定日志等级
     
用例
+++++++++
.. Note:: 
    测试项目：SpringDemo

- 当需要将应用绑定到云端项目 SpringDemo 时：
    
.. code-block:: bash
    
    java -javaagent:/path/to/agent.jar -Ddongtai.app.name=SpringDemo -jar SpringDemo.jar

- 当需要排查 Agent 报错问题或者二次开发 Agent 时需要本地调试：

.. code-block:: bash

    java -javaagent:/path/to/agent.jar -Ddongtai.debug=true -jar SpringDemo.jar

- 当启动 Agent 影响了应用的运行，需要设置 Agent 延迟启动时间，以 15 秒为例：

.. code-block:: bash

    java -javaagent:/path/to/agent.jar -Diast.engine.delay.time=15 -jar SpringDemo.jar

- 当排查 agent 异常或者研究字节码转换原理时，在目录 ``/tmp/class`` 查看转换后的字节码文件：

.. code-block:: bash

    java -javaagent:/path/to/agent.jar -Diast.dump.class.enable=true -Diast.dump.class.path=/tmp/class -jar SpringDemo.jar

- 当前网络无法访问洞态云端需要设置HTTP代理，以设置代理 10.100.100.1:80 为例：

.. code-block:: bash

    java -javaagent:/path/to/agent.jar -Diast.proxy.enable=true -Diast.proxy.host=10.100.100.1 -Diast.proxy.host=80 -jar SpringDemo.jar

- 当需要设置检测能力为 hunter/normal 时（hunter 模式的使用场景：代码审计，normal 模式使用场景：企业内部检测漏洞）：

.. code-block:: bash

    java -javaagent:/path/to/agent.jar -Diast.mode=hunter/normal -jar SpringDemo.jar


