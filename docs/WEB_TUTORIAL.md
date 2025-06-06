# [123云盘](https://www.123pan.com) 无限制分享工具（Web界面使用教程）

## 目录

- [123云盘 无限制分享工具（Web界面使用教程）](#123云盘-无限制分享工具web界面使用教程)
  - [目录](#目录)
  - [连接网络、下载安装浏览器](#连接网络下载安装浏览器)
  - [打开网页](#打开网页)
    - [访问链接](#访问链接)
    - [界面截图](#界面截图)
  - [`从私人网盘导出` 功能](#从私人网盘导出-功能)
    - [`从私人网盘导出` 界面截图](#从私人网盘导出-界面截图)
    - [参数介绍](#参数介绍)
    - [运行结果截图](#运行结果截图)
    - [运行结果参数介绍](#运行结果参数介绍)
  - [`导入到私人网盘` 功能](#导入到私人网盘-功能)
    - [`导入到私人网盘` 界面截图](#导入到私人网盘-界面截图)
    - [参数介绍](#参数介绍-1)
    - [运行结果截图](#运行结果截图-1)
    - [运行结果参数介绍](#运行结果参数介绍-1)
  - [`从分享链接导出` 功能](#从分享链接导出-功能)
    - [`从分享链接导出` 界面截图](#从分享链接导出-界面截图)
    - [参数介绍](#参数介绍-2)
    - [运行结果截图](#运行结果截图-2)
    - [运行结果参数介绍](#运行结果参数介绍-2)


## 连接网络、下载安装浏览器

- 基础问题，不解释。

## 打开网页

### 访问链接

- 如果您是自己本地部署，访问链接请见控制台窗口，例如：

    ```shell
    (py312) d:\123Pan-Unlimited-Share>python web.py
    * Serving Flask app 'web'
    * Debug mode: off
    WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
    * Running on all addresses (0.0.0.0)
    * Running on http://127.0.0.1:33333        <<< 访问连接在这里
    * Running on http://198.18.0.1:33333       <<< 访问连接在这里
    Press CTRL+C to quit
    ```

- 也可以使用本人部署的网页（服务器很渣，建议自己部署使用）：[>>> 点击这里进入 <<<](http://222.186.21.40:33333/)。

- 您也可以使用他人部署的网站，请见：（没有🥺）

### 界面截图

- 主界面如下

    ![](images/index_page.png)

## `从私人网盘导出` 功能

### `从私人网盘导出` 界面截图

- 界面如下

    ![](images/export_page.png)

### 参数介绍

- ⚠️**特别说明**：网站使用 Cookies 在浏览器**本地存储**你的用户名密码，以此实现每次刷新页面时自动填入账号密码的功能，**网站不会记录你的账号密码数据**。此外，请不要在公共电脑上使用。

- **账号**：填写你123云盘的手机号/邮箱。

- **密码**：填写你123云盘的密码。

- **根目录名 (分享名)**：例如：`ABC`，后续下载的文件将会以 `ABC.123share` 命名，别人导入时，会以 `ABC` 作为导入的根目录文件名）。

- **文件夹ID**：填写你要分享的文件夹的ID，获取方式请参考：[>>> FAQ <<<](https://github.com/realcwj/123Pan-Unlimited-Share#faq)。

- **加入资源共享计划**：勾选后，本次导出的资源将在审核后对公众可见。

### 运行结果截图

- **⚠️请耐心等待程序运行，运行速度取决于分享的文件总数。**

- 界面如下

    ![](images/export_result_page.png)

### 运行结果参数介绍

- **操作结果**：这里会实时显示当前导出进度。

- **分享码**：分享码，用于分享给他人。

## `导入到私人网盘` 功能

### `导入到私人网盘` 界面截图

- 界面如下

   ![](images/import_page.png)

### 参数介绍

- ⚠️**特别说明**：网站使用 Cookies 在浏览器**本地存储**你的用户名密码，以此实现每次刷新页面时自动填入账号密码的功能，**网站不会记录你的账号密码数据**。此外，请不要在公共电脑上使用。

- **账号**：填写你123云盘的手机号/邮箱。

- **密码**：填写你123云盘的密码。

- **选择.123share 文件（可选）**：选择你要导入的 `*.123share` 文件。注意：文件名中的 `*` 部分会作为导入的根目录文件名。

    选择文件后，将自动填入下方的 `分享码` 和 `根目录名`，您也可以不选择文件，手动填入下方的信息。

- **分享码**：他人分享给你的分享码。

- **根目录名**：例如：`ABC`，后续导入的文件将会以 `ABC` 作为导入的根目录文件名）。

- **从公共资源库选择**：即大家共享出来的资源，不解释。

### 运行结果截图

- **⚠️请耐心等待程序运行，运行速度取决于接收的文件总数。**

- 界面如下

   ![](images/import_result_page.png)

- 导入后，请去123云盘查看是否导入成功。

    ![](images/import_check.png)

### 运行结果参数介绍

- **操作结果**：这里会实时显示当前导出进度。

## `从分享链接导出` 功能

### `从分享链接导出` 界面截图

- 界面如下

  ![](images/link_page.png)

### 参数介绍

- **分享链接 Key**：例如，分享链接：`https://www.xxx.com/s/abcd-efg`，此处填写末尾的 `abcd-efg` 部分。

    **您也可以粘贴完整链接，例如：`https://www.xxx.com/s/abcd-efg`，浏览器会自动尝试解析。**

- **分享密码 (提取码)**：填写分享密码，例如，`ABCD`，如果没有密码就不填

- **分享文件夹ID**：保持默认 `0` 即可，代表导出整个分享链接。

- **根目录名 (分享名)**：例如：`ABC`，后续下载的文件将会以 `ABC.123share` 命名，别人导入时，会以 `ABC` 作为导入的根目录文件名）。

- **加入资源共享计划**：勾选后，本次导出的资源将在审核后对公众可见。

### 运行结果截图

- **⚠️请耐心等待程序运行，运行速度取决于分享的文件总数。**

- 界面如下

    ![](images/link_result_page.png)

### 运行结果参数介绍

- **操作结果**：这里会实时显示当前导出进度。

- **分享码**：分享码，用于分享给他人。