---
ms.localizationpriority: medium
ms.openlocfilehash: c804bdd39ebc2c460aa261355703b50ba530b197
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289515"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->
<!--- # Introduction --->

Microsoft Graph连接器允许你将你自己的数据添加到 Microsoft Graph，并可以支持各种Microsoft 365体验。

此 .NET Core 应用程序演示如何使用 Microsoft Graph 连接器 API 创建客户连接器并使用它来Microsoft 搜索。 本教程使用 Contoso 设备修复组织的示例数据设备部件清单。

## <a name="how-does-the-sample-work"></a>示例如何工作？

此示例创建一个Windows桌面应用，该应用从 Microsoft 标识平台 获取令牌，并使用它向 Microsoft Graph 连接器 API 发送请求。 连接器 API 将在验证访问权限后发送其响应。

![显示应用Windows令牌并使用它访问 Microsoft Graph 连接器 API 的关系图](images/connectors-images/build1.png)

## <a name="prerequisites"></a>先决条件

* 在Visual Studio计算机上安装带[.NET Core 3.1 SDK](https://www.microsoft.com/net/download/core)的[2019](https://visualstudio.microsoft.com/)版本。
* 确保你有个人 Microsoft [帐户或](https://signup.live.com/)工作或学校帐户。
* 使用下面的 [命令将实体框架核心](/ef/core/miscellaneous/cli/dotnet) 工具安装为全局工具：

    ```dotnetcli
    dotnet tool install --global dotnet-ef
    ```

* 安装用于更新 SQLite 数据库的工具。 例如，适用于 [SQLite 的 DB 浏览器](https://sqlitebrowser.org/)。
* 从 **ApplianceParts.csv** 示例存储库 [下载文件](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv)。

> [!TIP]
> 从网站下载文件GitHub转到项目的顶级。 在右侧绿色 **代码** 下载按钮中，选择"**下载 ZIP"。** ZIP 文件将包含存储库的内容。
