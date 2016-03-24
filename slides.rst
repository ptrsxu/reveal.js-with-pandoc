===========
主标题
===========

:title: 主标题
:subtitle: 副标题
:author: Peter Xu
:date: 2016-03-20


第一张幻灯片
------------

可以支持中文。请看列表

-  第一项
-  第二项

   -  `Google <http://google.com>`__
   -  还可以在\ http://rvl.io\ 上在线编辑slides

-  第三项 数学公式 :math:`\frac{x^2}{2}`

第二张幻灯片
------------

尝试逐项出现条目

.. raw:: html

   <ul>
   <li class="fragment">第一项</li>
   <li class="fragment">第二项</li>
   </ul>

可以没有标题

.. figure:: fig/html5.png
   :alt: 图片说明

   图片说明

表格
----

+--------+--------+
| name   | type   |
+========+========+
| 张三   | 好人   |
+--------+--------+
| 李四   | 坏人   |
+--------+--------+

表格的样式我放在/css/custom.css里了

变量
----

下面两个是可以在命令行中定义的变量

-  theme
-  transition

以linux下的shell脚步为例：

.. code:: bash

    pandoc -t html5 --template=template-revealjs.html \
        --standalone --section-divs \
      --variable theme="beige" \
      --variable transition="linear" \
      slides.md -o slides.html

windows下的情况请看本项目repo中的\ `bat文件 <https://github.com/yanping/reveal.js-with-pandoc/blob/gh-pages/build.bat>`__
