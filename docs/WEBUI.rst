WEBUI 网页界面
=================

``Typhon`` 内置一个轻量的 WebUI（仅使用 Python 标准库），用于在浏览器中调用 :func:`~Typhon.bypassRCE` / :func:`~Typhon.bypassREAD`。

启动方式
--------

如果你通过 pip 安装了 ``typhonbreaker``，可以直接启动：

.. code-block:: bash

   typhonbreaker webui

默认监听 ``127.0.0.1:6240``，浏览器打开： ``http://127.0.0.1:6240`` 。

参数
----

``webui`` 支持以下参数：

.. code-block:: bash

   typhonbreaker webui --host 0.0.0.0 --port 6240

.. warning::

   WebUI 默认绑定到 ``127.0.0.1``。如果你运行在服务器上，请自行做好访问控制/防火墙配置。

Docker
------

本仓库提供用于构建 WebUI 镜像的 ``Dockerfile``，你可以用 compose 直接启动：

.. code-block:: bash

   docker compose up --build

