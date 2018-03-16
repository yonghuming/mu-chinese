Mu的架构
-----------------

This section provides a high level overview of how the various parts of Mu
fit together.
本章从宏观上带领大家认识Mu编辑器不同部分的代码是如何协同工作的.

核心概念
============

The key concepts you should know are:
你应当了解的核心概念有:


* Mu通过`PyQT5 framework <https://riverbankcomputing.com/software/pyqt/intro>`_ (让Python可以使用 `Qt <https://www.qt.io/>`_ 个性化界面接口)来编写软件界面.
* Mu是一个模态编辑器:Mu编辑器的行为跟根据模式的不同有所变化
* 有一些核心功能和行为无论在什么模式下都是可用的不变的,无论什么模式
* 代码编辑区是基于 `Scintilla <http://www.scintilla.org/>`_ 开发的组件
* Mu通过使用python标准的 ``gettext`` 模块和工具来实现国际化
*mU的代码并不多,而且有详尽的文档,并且经过100%的测试.

代码组织结构
==============

The code is found in the ``mu`` directory and organised in the following way:
核心代码在 ``mu`` 目录,并且按照如下方式组织:

* 通过 ``app.py`` 来创建和配置应用
* ``logic.py`` 提供了Mu编辑器基本工作逻辑
* ``contrib`` 目录保存了未打包的第三方代码
* Python 3调试器包含了命令空间 ``debugger`` 中的一个调试器客户端和调试器运行期. 关于调试器的工作细节可以查阅 :doc:`debugger`
* ``interface.main`` 模块中的 ``window`` 负责与UI界面进行交互. ``interface.main`` 命名空间下的其他模块包含了 ``Window`` 类中用到的订制界面的代码.
* Mu编辑器国际化相关的资源保存在 ``locale`` 目录下. 查阅 :doc:`translations` 文档了解细节.
* ``modes`` 命名空间下包含了许多模式.所有的模式都继承自 ``BaseMode`` 类,关于模式的细节可以参考 :doc:`modes`
* ``resources`` 目录下保存了主题用到图形资源,字体和CSS样式表.

所有的类,方法和函数都有 *可读性极高的* 注释.
所有的注释都被导出到 :doc:`api` 文件.

:doc:`tests` is in the ``test`` directory and filenames for tests relate
directly to the file they test in the Mu code base. The module / directory
structure mirrors the organisation of the Mu code base. We use PyTest's assert
based unit testing. All tests have a comment describing their intent.

The documentation you're reading right now (i.e. that written for developers)
is found in the ``docs`` directory. We use `Sphinx <http://www.sphinx-doc.org/en/stable/>`_
to write our docs and host them on `ReadTheDocs <https://mu.readthedocs.io/en/latest/>`_.
Other documentation (tutorials, user help and so on) is on :doc:`website`.

``utils`` 包含了Mu编辑器生成API文档,代码自动完成和代码提示功能需要的不同的脚本.

The other assets in the root directory of the project are mainly for
documentation (such as our Code of Conduct), configuration (for testing) or
packaging for various platforms (see :doc:`packaging`).


If you want to make changes please read :doc:`contributing`.
