.. mu documentation master file, created by
   sphinx-quickstart on Thu Dec 24 16:24:33 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Mu: Python代码编辑器
========================

.. image:: logo.png

.. note::

    **本文档并非面相Mu的普通用户**. 而是一份给哪些想让Mu变得更好的软件开发人员的指南. 
    阅读我们的 :doc:`setup` 文档获取入门的一些技术细节.

    For tutorials, how-to guides and user related discussion, please see the
    project's website for users of Mu at: https://codewith.mu/
    如果你需要的是教程,以及软件使用指导以及用户相关的讨论,请访问我们为Mu用户准备的项目
    网站:https://codewith.mu/

What?
-----

Mu is a very simple Python editor for kids, teachers and beginner programmers.
It's written in Python and works on Windows, OSX, Linux and Raspberry Pi.
Mu是为孩子,教师和编程初学者准备的简单的Python编辑器.用Python语言开发并且能够在Windows,
苹果系统,Linux操作系统以及树莓派上运行.

    "[Papert] realized, 'Oh, we could take the real content out here as a
    version in the child's world that is still the real thing.' It's not a fake
    version of math. It's kind of like little league, or even T-ball. In sports
    they do this all the time. In music, they do it all the time. The idea is,
    you never let the child do something that isn't the real thing -- but you
    have to work your ass off to figure out what the real thing is in the
    context of the way their minds are working at that developmental level."
    -- `Alan Kay <https://www.fastcompany.com/40435064/what-alan-kay-thinks-about-the-iphone-and-technology-now>`_

Mu aspires to be "the real thing" as a development environment for beginner
programmers taking their first steps with Python.
Mu致力于成为初次接触Python的编程入门人员的"真正的东西",真实的开发环境.

As a rule of thumb, if you're able to ask "why doesn't Mu have [feature X]?"
then you're probably too advanced for using Mu as a development environment. In
which case, you should graduate to a more advanced editor.
总而言之,你也许会问,为什么Mu没有这个功能或者那个功能,那么可能是高级开发人员而没有必要
使用Mu作为开发环境了.这样的话,你就需要使用一个更加高级的编辑器.

Why?
----

There isn't a cross platform Python code editor that is:
没有任何一个跨平台的Python代码编辑器能够做到:

* Easy to use;简单易用;
* Available on all major platforms;在所有主流平台可用;
* Well documented (even for beginners);文档齐全(哪怕是针对新手);
* Simply coded;代码简介;
* Currently maintained; and, 一直维护,并且
* Thoroughly tested.经过了完全的代码测试.

Mu addresses these needs.Mu有以下需求.

Mu was originally created as a contribution from the
`Python Software Foundation <http://python.org/psf>`_
for the BBC's `micro:bit project <http://microbit.org/>`_. Many people asked if
Mu could be turned into a generic beginner's code editor and, thanks to the
wonderful support of the `Raspberry Pi Foundation <http://raspberrypi.org/>`_
the work needed to make such changes was done over the summer of 2017.

Mu最最初是`Python软件基金会 <http://python.org/psf>`_
为BBC的 `micro:bit项目 <http://microbit.org/>`_开发的. 很多人都好奇Mu能否成为一个通用
的入门级代码编辑器,感谢`树莓派基金会<http://raspberrypi.org/>`_
的大力支持,这些工作在2017年的时候完成了.

How?
----

Mu's outlook is:
Mu界面设计原则:

* Less is more (remove all unnecessary distractions);简胜繁(去掉不必要的功能)
* Keep it simple (so Mu is easy to understand);保持简洁(因此Mu易于理解);
* Walk the path of least resistance (Mu should be easy to use);路径阻力最小(Mu应该简单易用);
* Have fun (learning should be a positive experience).有趣(学习是积极的体验);

Mu's own code is simple, clearly organised and well tested. It's copiously
commented and mostly found in a few obviously named Python files.
Mu的代码非常简洁优雅,结构清晰并且经过了良好的代码测试.注释良好并且由少量明明清晰的
Python文件组成.

This has been done on purpose: we want teachers and kids to take ownership of
this project and organising the code in this way aids the first steps required
to get involved.
这是我们的设计目标支持:我们希望教师和学生能够参与这个项目,并且以能够帮助他们迈出参与
项目的第一步.

If you're looking for ways to get involved check out some of the
:doc:`first-steps` for new contributors.
如果想知道如何参与我们的项目,可以查看我们的文档 :doc:`first-step`,这是为新的贡献者
准备的文档.

Furthermore, we put our users at the centre of our development work. Extensive
interviews with teachers, observations of lessons and exceptionally clear and
helpful feedback from the education team at the Raspberry Pi Foundation 
(perhaps the most successful computing in education project in history) have
informed the design choices for Mu.
而且,在开发过程中,我们始终以用户为核心.与大量的老师进行座谈,观察课堂教学,并且从树莓派
基金会(可能是史上最成功的教育项目)教育组获取大量非常清晰和有用的反馈,这些给我们带来了
清晰的设计选择.

Who?
----

**你!**

Contributions are welcome without prejudice from *anyone* irrespective of
age, gender, religion, race or sexuality. If you're thinking, "but they don't
mean me", *then we especially mean YOU*. Good quality code and engagement
with respect, humour and intelligence wins every time.
我们欢迎 *任何人* 参与项目,我们不带有任何偏见,无论你的年龄,性别,宗教信仰,种族或者
性取向,我们都欢迎你参与项目. 如果你觉得,我们希望的不是你,"我们真的是希望你参与"

阅读文档 :doc:`contributing` 也许你会迈出第一步 :doc:`first-steps`.

We want the Mu community to be a friendly place. Therefore, we expect
contributors to follow our :doc:`code_of_conduct`.
我们希望Mu社区能够成为一个充满友善的社区.因此,我们希望贡献者们能够遵守我们的 :doc:`code_of_conduct`
代码协议.

内容:
---------

.. toctree::
   :maxdepth: 2

   contributing.rst
   code_of_conduct.rst
   setup.rst
   first-steps.rst
   user-experience.rst
   architecture.rst
   modes.rst
   translations.rst
   debugger.rst
   tests.rst
   packaging.rst
   website.rst
   api.rst
   authors.rst
   changes.rst
